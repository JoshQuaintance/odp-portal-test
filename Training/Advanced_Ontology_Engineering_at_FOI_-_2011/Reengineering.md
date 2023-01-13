__Problem__:
Exercise on reengineering DBs to OWL/RDF.




__Solutions__:



###   Reengineering and Refactoring using Semion


In this exercise you will use the Semion tool to reengieer a database table from an example database into RDF, and then to refactor it so that the data is expressed using the FOAF vocabulary.


__The database:__


host: mysql315.loopia.se


user name: d2r@o45820


password: (given at the course)


database name: ontology\_se\_db\_2


Content: The database contains information about a past ISWC conference, and in one table called "persons" there is information about the people that organized or attended the conference.


__The Semion rule language syntax:__


The complete Semion rule syntax can be found [here](http://www.ontologydesignpatterns.org/ont/training/foi/SemionRules.pdf "http://www.ontologydesignpatterns.org/ont/training/foi/SemionRules.pdf"), however you don't need it for the first part of this exercise.


  

__Task 1:__


Your task is to use Semion to express this data in terms of the FOAF vocabulary, at the following URI: [http://xmlns.com/foaf/0.1/](http://xmlns.com/foaf/0.1/ "http://xmlns.com/foaf/0.1/")


  

Start Semion from the commandline as follows (from the directory where you unpacked Semion):


Mac:
java -jar -Xmx512m -XstartOnFirstThread it.cnr.istc.semion.tool-0.6-SNAPSHOT.one-jar.jar 


Windows: 
java -jar -Xmx512m it.cnr.istc.semion.tool-0.6-SNAPSHOT.one-jar.jar


  

When the tool starts, the following procedure lets you do the first syntactical transformation (reengineering):



* When the tool starts you see the workspace on the left, with an example project called "test". Open the text project, and right-click on the "Data sources" icon.
* Select "New", "Data source", and "Relational database".
* In the dialogue that appears, give the database a name, e.g. "ISWC", and select the type "MySQL". Enter the host given above, and the port 3306. Database name and username according to above, and the password given to you on site. Finally, set a URI for your new data that will be the result of the reengineering, e.g. "[http://example.org/myISWCdata/](http://example.org/myISWCdata/ "http://example.org/myISWCdata/")" and then click on "finish".
* Double click on your new datasource in the Project Explorer, so that a tab appears to the right with information about the DB.
* At the bottom-left of the new tab, you can see all the tables of the database. Here you can select what tables of the DB you want to work with. Select the "persons" table, and click on "Extract data" in order to start the reengineering process, i.e. the syntactic transformation step.
* In the source code tab (bottom) you can see the result of the transformation. The table and its data is now described according to the relational database metamodel of Semion. In the SPARQL tab you can also query this data.
* However, so far we have only transformed the source syntactically, so now we want to align the data to the FOAF ontology. Start by right-clicking on the data source in the Project Explorer, and select New, Alignment.
* In the dialogue that appears, you have to first give the alignment a name. Then you can either select to simply use the OWL vocabulary itself as the basis for your alignment, or you can choose to add your own ontology. We want to align our data to the FOAF vocabulary, hence click on the "new ontology" button.
* First you give the ontology and ID and a name (both can be anything you choose, but the ID needs to be unique for the workspace). Then provide the online URI of the ontology, i.e for FOAF you input [http://xmlns.com/foaf/0.1/](http://xmlns.com/foaf/0.1/ "http://xmlns.com/foaf/0.1/") Then click Finish.
* Now the ontology appears in the drop-down list under the name you gave it. Select it and then click on Finish.
* In the Project Explorer, under your datasource, and the Alignment subcategory, you alignment should now appear. Double click on it to open its related tab.
* In the overview you can see any annotations related to the ontology you have chosen to align to. And in the SPARQL tab you can query your alignment, however, currently it is empty. Instead go to the Alignment Rules tab. This is where you can now create your alignment, i.e. the transformation rules that brings the data from the RDF model of your database into something expressed using the FOAF model instead.
* We now want to identify all the persons in the database and set them as instances of FOAF person.
	+ If you go back to the tab showing the database, and execute the example SPARQL query in the SPARQL tab, you can see all the RDF triples that were generated. If you scroll down the list you will find the actual data of the persons table, expressed as record instances. For instance, for each entry in the persons table there are two triples looking like this: dbSchema:persons\_record\_x rdf:type dbs:Record and dbSchema:persons\_record\_x dbs:isRecordOf dbSchema:persons\_table.
	+ You should write rules that fetch each such persons\_record\_x and takes the data it has associated, i.e. through the dbSchema:persons\_record\_x\_datum\_x dbs:isDatumOf dbSchema:persons\_record\_x, and extracts its values, e.g. the first and last name of each person as properties of the new FOAF person you are creating.
* Go back to the tab of the alignment, and select the Alignment Rules tab.
* At the top you see the list of rules currently inserted in this alignment (at the moment it is empty). Click on the Add-button below the table.
* Give a name to the rule, e.g. foaf\_person. Then copy the following text as the content of the rule and click Finish:
	+ has(dbs:isRecordOf, ?person, dbSchema:persons\_table) . has(dbs:isDatumOf, ?y, ?person) . has(dbs:bindsToColumn, ?y, dbSchema:persons\_FirstName-column) . values(dbs:hasContent, ?y, ?fname) . has(dbs:isDatumOf, ?z, ?person) . has(dbs:bindsToColumn, ?z, dbSchema:persons\_LastName-column) . values(dbs:hasContent, ?z, ?lname) -> is(foaf:Person, ?person) . values(foaf:firstName, ?person, ?fname) . values(foaf:lastName, ?person, ?lname)
	+ This may seems like a very complex rule, but lets break it down to see what it means. "has" is the keyword for object property assertions, "is" indicates a rdf:type relation, and "values" indicates a data property assertion. The condition then consists of three parts:
		- has(dbs:isRecordOf, ?person, dbSchema:persons\_table) - this matches triples that says that something (the variable ?person) is a record of the table person of the reengineered database, i.e. ?person is a row in the persons table.
		- has(dbs:isDatumOf, ?y, ?person) . has(dbs:bindsToColumn, ?y, dbSchema:persons\_FirstName-column) . values(dbs:hasContent, ?y, ?fname) - this gets the the entry in that row that is the first name, and extracts the value into the variable ?fname
		- has(dbs:isDatumOf, ?z, ?person) . has(dbs:bindsToColumn, ?z, dbSchema:persons\_LastName-column) . values(dbs:hasContent, ?z, ?lname) - does the corresponding thing for the lastname
	+ Then look at the consequent, i.e. what happens if we find something that fulfills the conditions above:
		- is(foaf:Person, ?person) - set the record we found as an instance of foaf:Person, i.e. we align our data to the foaf ontology
		- values(foaf:firstName, ?person, ?fname) - relate that person instance through the foaf:firstName property to the string value we have extracted
		- values(foaf:lastName, ?person, ?lname) - same for the lastname
* After clicking Finish the rule should appear in the table of rules. Now click on Run Refactoring, to apply the rule to our RDF data.
* Wait until the processing has finished and then go to the SPARQL tab of the alignment. Run the default query that gets all the triples generated by the alignment.
* Now you should see a set of triples representing a set of instances of foaf:Person, each with a foaf:firstName and foaf:lastName - this is our refactored dataset!


  

If you have time left, proceed to write your own rules to extract more data from the database. For instance, you could write additional rules that extract more of the information about people from the persons table!


Otherwise, proceed to try out the D2R virtual RDF server below.



###   Using D2R


Now, you should try to use D2R to instead create a runtime mapping to the DB, so that you can query the DB using SPARQL.


__Task 2:__


Use the same database as above, and run the following tutorial:
[http://sw.cs.technion.ac.il/d2rq/tutorial](http://sw.cs.technion.ac.il/d2rq/tutorial "http://sw.cs.technion.ac.il/d2rq/tutorial")


The example data is already loaded into the database, but you have to edit the example mapping to reflect the details of the database above. Then you can run the D2R server (with the mapping file in the same directory) and try accessing the DB through SPARQL in your browser.


How do the results compare to the ones we got with Semion?





Retrieved from "[http://ontologydesignpatterns.org/wiki/Training:Advanced\_Ontology\_Engineering\_at\_FOI\_-\_2011/Reengineering](../../Category/ProposedReengineeringOP)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [Exercise](../../Category/Exercise "Category:Exercise")