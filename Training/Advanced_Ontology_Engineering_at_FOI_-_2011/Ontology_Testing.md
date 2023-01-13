__Problem__:
The task of the exercise is presented at the  [bottom of this page](../../Training/Advanced_Ontology_Engineering_at_FOI_-_2011/Ontology_Testing.md#Tasks "Training:Advanced Ontology Engineering at FOI - 2011/Ontology Testing"). First, read through the instructions below.




__Solutions__:



* Solution ideas are available  [here](../../Training/Advanced_Ontology_Engineering_at_FOI_-_2011/Ontology_Testing/Testing_Solution.md "Training:Advanced Ontology Engineering at FOI - 2011/Ontology Testing/Testing Solution"), do not open until end of the exercise!


__Instructions for the exercise:__


Below you find general descriptions of the three testing methods that you will apply during this exercise, the same as you hear about in the lecture. Read through the descriptions of the methods, then proceed with solving the tasks that are described at the bottom of this page. Try to make sure you have enough time to try out all three methods, i.e. if you don't have time to complete the testing using one method, proceed anyway so that you have time to try all three. 
Don't forget to document what you are doing while you solve the task!


  




##   Method 1: Unit testing through SPARQL queries


Parts of the ontology requirements are usually expressed as competency questions (CQs), i.e. natural language questions that the ontology should be able to provide answers to. One way to practically allow the ontology to answer such questions is to reformulate them as SPARQL queries, in order to retrieve the appropriate facts from the knowledge base. This also introduces a way of testing your ontology module!


Assuming that your ontology attempts to solve the two CQs, CQ1 and CQ2. Then each of those should be possible to formulate as a SPARQL query, Q1 and Q2, over the ontology module, such that the retrieved instances and/or literal values constitute the answer to the CQs. Q1 and Q2 could be considered as unit tests for the module, since they assure that the requirements CQ1 and CQ2 are actually met. 


This method of testing contains the following steps:



1. Retrieve (and read) all the CQs that are realized by the module in question.
2. Select one CQ to start with.
3. Reformulate it as a SPARQL query over the ontology module, using the classes, properties, and instances that the module provides. Each CQ requires one unit test, which can usually be realized as one single SPARQL query.
4. For each unit test, i.e. each SPARQL query, create a new "test case"-module importing the module to be tested, and add facts to it. The test data can come from the initial customer story, it can be provided by a domain expert, or it has to be "invented" by the developer. Make sure the test data covers the classes and properties that are present in the SPARQL query in question (created in step 3).
5. For each SPARQL query developed according to step 3 decide, based on the test data added in 4, what a successful test should return, i.e. for each SPARQL query, what instances and/or literal values should be returned?
6. Run the SPARQL query over the respective "test case"-module and record the results.
7. Compare the actual results (from step 6) to the expected ones (from step 5), and decide if the test was successful or not.
8. For any unsuccessful tests, analyze the reason for the failure by inspecting the ontology. Document the error/problem, so that it can be resolved by you or other ontology developers.
9. Document your "test case" module by annotating it, so that anyone who reuses it in the future knows what requirements you were testing, what was the input, i.e. test data, the expected output, and the actual output of the test. Additional metadata can also be useful, such as who performed the test, when, and using what reasoner.
10. Proceed with the next CQ (i.e. go back to step 2)!


  

__Example__
I have built an ontology for the theater domain. In the ontology there is a module modelling plays and theater productions, that realize the CQ "What play is this production based on?", i.e. modelling the distinction between plays (as abstract literary works) and theater productions (where an ensemble has set up a certain play). The module specializes the Information Realization ODP and contains the classes "Play" (as a subclass of InformationObject) and "Production" (as a subclass of InformationRealization), as well as the properties "producesPlay"/"playProducedIn" as subproperties of the pattern properties. To test this using the method described above, I formulate the CQ as the following SPARQL query:




```
  SELECT ?production ?play
  WHERE { ?production :producesPlay ?play . }

```

Next, I create a new empty ontology, where I import the module about plays and productions. I add some concrete instances of plays and productions, and relate them through the available properties, for instance triples like _merchantOfVeniceProduction producesPlay merchantOfVenice_. I then list the "correct answers" that the SPARQL query should return, in the case of the triple above it would be the variable bindings ?production - merchantOfVeniceProduction and ?play - merchantOfVenice. Then I run the query and check that that is actually what I get. Most often you will notice that it is actually at query-writing time you will discover the mistakes, i.e. things that makes it impossible or at least difficult to pose that query, however, it is still important to add instances and actually run the query as well, it gives you empirical evidence that the requirement is actually solved.


  




##   Method 2: Performing inferences


Although CQs express what information the ontology should be able to provide, they usually do not say exactly how this information is produced, i.e. if it is input into the ontology explicitly as assertions or how it can be produced from other facts through some inference mechanism. Therefore an ontology can have additional requirements complementing the CQs, or explaining complex CQs, describing some desired inferences that the ontology should support. For instance, in an ontology about people we may define the class "parent" and say that any person who has at least one child is a parent. If we are not expecting the information about being a parent to be explicitly entered into the ontology's knowledge base, we may instead expect it to be derived from the presence of "hasChild" relations. This is a reasoning requirement that requires the ontology to include the appropriate axioms to make this inference. 


To test the desired inferences of the ontology module, follow these steps:



1. Inspect the explicit reasoning requirements that you can find among the requirements of the module, if any. Also, determine if there are any implicit reasoning requirements, i.e. reasoning requirements that are implied by complex CQs and that should be added to the set of requirements. This may include some interaction with the customer or a domain expert, if the requirements are ambiguous.
2. For each such requirement (in the list from step 1), list what is the input and expected output, e.g. given some example facts taken from the story or "invented" by you, what facts (triples) need to be present before actually running the inference engine, and what facts (triples) can be produced by the inference procedure.
3. Create one new "test case"-module for each reasoning requirement, import the module to be tested in each one, and add facts to it. For each reasoning requirement in the list from step 1, add some facts that can be considered as the "input" to the reasoning process (according to the result of step 2).
4. List the expected inferences that should be made based on your test data, i.e. the expected test output, for each test module.
5. Run an OWL reasoner over the "test case"-modules and record the results.
6. Compare the actual results (from step 5) with the expected ones (from step 4), and decide if the test of each reasoning requirement was successful or not. A test is successful if it produces the expected inferences, and no harmful or unnecessary side-effects, i.e. no additional inferences that add undesirable or incorrect facts to the knowledge base.
7. For any unsuccessful tests, analyze the reason for the failure by inspecting the ontology. Document the problem, so that it can be solved by you or by other ontology developers.
8. Document your "test case" module by annotating it, so that anyone who reuses it in the future knows what requirements you were testing, what was the input, the expected output, and the actual output of the test. Additional metadata can also be useful, such as who performed the test, when, and using what reasoner.
9. If you still did not test all the reasoning requirements, explicit of implicit, start over from step 2.


  

__Example__
I have built an ontology for the theater domain. In the ontology there is a module modeling persons, including their roles as actors and authors of plays. The requirements include a reasoning requirement, saying that I want to be able to classify persons as either authors or actors, based on if on one hand they have written a play or on the other hand have participate in any production. The module contains the classes "Person", with "Author" and "Actor" as subclasses, "Play" and "Production". The property "wrote" relates a person to a play, and the property "playsIn" relates a person to a production. Additionally I have defined Author as equivalent to instances that are persons and wrote some play, and similarly Actor as equivalent to instances that are persons and playsIn some production. 


The input needed for this reasoning requirement are triples relating persons to either plays or productions through the "wrote" and "playsIn" properties respectively. The expected output are triples of the form <person-instance> rdf:type :Actor/:Author. I proceed to create a new test case module, i.e. an empty ontology, where I import the module described above. Then I add a number of triples using the "wrote" and "playsIn" properties, e.g. _Anne playsIn merchantOfVeniceProduction_. I list the expected inferences, i.e. for the example triple it would be the new triple _Anne rdf:type Actor_. I run the reasoner and check that this triple is actually inferred, and that no other strange things appear as inference results. 


  




##   Method 3: Performing "stress tests"


Although the ability to perform correct inferences, and provide the resulting information as a result of queries, allow us to see that the ontology actually realizes its requirements, another important characteristic of an ontology is to allow as few erroneous facts and/or inferences as possible. A high-quality ontology allows exactly the desired inferences and queries, while avoiding to produce irrelevant or erroneous side-effects. It may also be desirable to be able to check input data against some constraints and business rules. 


This category of testing can be compared to software testing, when usually a system is fed random data, data known to be incorrect, or data considered as "boundary values" for the input data, e.g. the extremes of value ranges, in order to check its robustness and capability to handle unexpected input. When dealing with ontologies, we are not evaluating how good error messages and recovery strategies are, as for software, but rather that erroneous facts and data is detected in the first place, or at least that it doesn't produce any unexpected side-effects. One way to detect such problems is by using the consistency checking facilities of a reasoning engine. A high-quality ontology facilitates the reasoner to detect inconsistencies in most cases when inappropriate or erroneous facts are entered. 


For instance, in a user models an ontology with the classes "female user" and "male user", where this information is going to be collected from a web form with a radio button, the classes should most likely be disjoint, i.e. since no user can select both alternatives from the form any given user can only be an instance of one class. After detecting such implicit requirements, or common sense constraints, and expressing them as contextual statements, they can be tested by entering obviously inconsistent facts, and checking that the reasoner is able to detect the inconsistency. 


To test this ability of the ontology, the following steps can be used:



1. Inspect the CQs and the explicit reasoning requirements of the ontology, and other constraints that have been explicitly expressed, i.e. the contextual statements. List the explicit requirements that should be tested, and also determine if there are any implicit requirements, e.g. additional constraints that can be derived from the requirements or the context, that should be added to this list. This may include some interaction with the customer, in order to determine what constraints are valid and important in the context. For each requirement to be tested, formulate the constraints it implies, e.g. a boundary on some value, or a restriction of class types etc.
2. For each of the constraints listed in step 1, determine if there is a range of values that constrain the acceptable input or output that should be allowed by the ontology. For each constraint, determine at least one case (literal value or fact) that lies outside of that range, or exactly constitutes the boundary, and what response would be expected to get from the reasoner given that input. Also, list any other kinds of erroneous input that could be tested, to check how well the ontology enforces those constraints.
3. Create a new "test case"-module for each of the intended tests, i.e. each constraint, by importing the module to be tested in each one and add facts to it (see next steps).
4. Add each of the cases listed in step 2 to its respective "test case"-module, and for each one run the reasoner and record the result.
5. For each run in step 5, check the result against the expected result determined in step 2, and decide if the test was successful or not. A test is successful if it produces the expected inferences, e.g. an inconsistency, and no harmful or unnecessary side-effects.
6. For any unsuccessful tests, analyze the reason for the failure by inspecting the ontology. Document the problem, so that it can be solved by you or other ontology developers. For these kinds of tests it is common that you also find limitations in the OWL language, i.e. things that you basically cannot express in a good way (e.g. given the open world assumption). Such things should be documented, and analyzed in the context of the overall software to use the ontology - perhaps you should use some special techniques for OWL, if these things are common, and very essential, or perhaps this checking can instead be performed in special-purpose software.
7. Document your "test case" module by annotating it, so that anyone who reuses it in the future knows what requirements you were testing, what was the input, the expected output, and the actual output of the test. Additional metadata can also be useful, such as who performed the test, when, and using what reasoner.
8. If you still did not test all the reasoning requirements, explicit or implicit, start over from step 2.


  

__Example__
I have built an ontology for the theater domain. In the ontology there is a module modeling persons acting in theater productions. There is also a contextual statement saying that each production has exactly one lead actor, i.e. the person that plays the main character of that drama. The module contains the classes "Person" and "Production", and the property "hasLeadActor" (which might be inferred based on a role playing situation, but that doesn't matter in this example). There is also an axiom stating that a production is related to exactly one person through the hasLeadActor property. 


For this contextual statement, and its realization as an axiom, I can see that "acceptable values" of the number of facts using the hasLeadActor property is 0 and 1 (0 is accepted since we have an open world assumption, so what is not entered might still be true). From this I can see that 2 would be an unacceptable number of facts using the hasLeadActor property, for the same production, i.e. this value is outside the range of acceptable input. If I explicitly state that those two instances of person (that the facts relate to) are different (owl:differentIndividuals) this should result in the reasoner discovering an inconsistency. I create a new ontology where I import the module described above, and add two facts about the same production, e.g. triples like _merchantOfVeniceProduction hasLeadActor Peter_ and _merchantOfVeniceProduction hasLeadActor Steve_. Then I assert that Peter and Steve are different individuals. Now, I run the reasoner on the module and check that it actually detects the inconsistency.



##   Tasks


1. Download [this ontology module](http://www.ontologydesignpatterns.org/ont/training/foi/musicindustry.owl "http://www.ontologydesignpatterns.org/ont/training/foi/musicindustry.owl"), and put it in the workspace of your ontology editor. Be sure you have SPARQL and reasoning support.
2. While you are working, __document what you are doing__ according to the instructions above, e.g. what requirement does each module test, what are the expected and actual results, and what errors are you able to find. You can record this in a text document on your laptop. Feel free to note down any additional comments you find relevant, e.g. about the testing methods themselves.
3. Try to plan your time, so that you try out all three methods, i.e. don't spend all your time on one method, if you don't have time to finish the testing using that method proceed with the other methods anyway! Approximately you should devote 20 minutes to each method.


  

Assume that the ontology was constructed with the following context in mind, and use the three methods described above to test the ontology. 


__Context:__ An online music database wishes to semantically represent their data about musicians, albums, and performances, in order to be able to provide better search functions to their users, i.e. by querying the knowledge base instead of using keyword-based queries. Below is an example of what they typically would like to store, and at the bottom you find the competency questions developed as requirements for the ontology.


Additionally, assume that the ontology requirements were based on the following user story:


__Story - music and bands:__ 
The current configuration of the “Red Hot Chili Peppers” is: Anthony Kiedis (vocals), Flea (bass, trumpet, keyboards, and vocals), Johs Klinghoffer (guitar), and Chad Smith (drums). 
The line-up has changed a few times during they years, Frusciante replaced Hillel Slovak in 1988, while Jack Irons was replaced by Chad Smith. 
In addition to playing guitars for Red hot Chili Peppers Frusciante also contributed to the band “The Mars Volta” as a vocalist for some time. 
In 2004, the Red Hot Chili Peppers started recording the album “Stadium Arcadium”. The album contains 28 tracks and was released in 2006. 
It includes a track of the song “Hump de Bump”, a funk-rock song composed in 2004. 


For testing you need the ontological requirements that were the basis of the ontology development, they can be found below. 
Consider that it is against these requirements that you are performing the testing, the scenario and context above only gives you some background information.
Also consider that you do not have to modify the ontology during this exercise, your goal is to identify modeling mistakes and document them. 


__Requirements:__


__Competency questions (CQs) and contextual statements of music and bands__



1. What instruments does a certain person play?
2. During what time did a certain band have what members?
3. What role does a certain person have in a certain band at a certain point in time?
4. What tracks are recordings of a certain song?
5. What is the genre, e.g., rock or pop, of this track?
6. What are the genres of this album?
7. During what time period was a certain album of a certain band recorded?
8. Who did participate in the recording of a certain album of a certain band?
9. When was a certain album released?
10. When was a certain song composed?


Contextual statement:



1. A recorded album has one or more genres
2. A track has only one genre
3. A track realizes only one song
4. Each band and each person is associated to at least one name


Reasoning requirement:



1. To identify (classify) bands into (multiple) genres based on the genres of their recorded tracks, e.g., a rock band has recorded some track in the genre "rock". In this system a band should be classified into a certain genre even if it has only one track of this genre.
2. To infer the genres of an album based on the genres of the tracks it contains




Retrieved from "[http://ontologydesignpatterns.org/wiki/Training:Advanced\_Ontology\_Engineering\_at\_FOI\_-\_2011/Ontology\_Testing](../../Training/Advanced_Ontology_Engineering_at_FOI_-_2011/Ontology_Testing.md)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [Exercise](../../Category/Exercise.md "Category:Exercise")