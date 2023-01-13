#  Tasks/References for Exemplary Ontologies


__Title:__ References for Exemplary Tasks


__Description:__ Currently, there is no good way for users to enter references with links and information about them. This is really a big deal, references are very important for this catalogue to be useful. Needs to have a solution that allows entering text as well as a link and to have them in a nice table. May also want a longer text description than a link name. May want a reference type too. 


  





* __Type__: Improvement
* __Posted by__: [MichaelUschold](../../User/MichaelUschold.md "User:MichaelUschold")
* __Status__: fixed


* __Priority__: High




__Sub-tasks__:
This task has no sub-tasks




[Development](../../Odp/Development.md "Odp:Development") | [Create new task](http://ontologydesignpatterns.org/wiki/Special:AddData/Task_Form?Task Template[SubmittedBy]=93.34.113.67).| [Add sub-task](http://ontologydesignpatterns.org/wiki/Special:AddData/Task_Form?parenttask=Tasks/References_for_Exemplary_Ontologies&Task Template[ParentTask]=Tasks/References_for_Exemplary_Ontologies&Task Template[SubmittedBy]=93.34.113.67) | [Add a comment at the bottom of this page](../index.php@title=Odp%253AAdd_comment&target=Odp%253ATasks%252F../../Odp/Tasks/References_for_Exemplary_Ontologies.md#New_comment "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_comment&target=Odp:Tasks/References_for_Exemplary_Ontologies#New_comment")
#####  25-02-2010 [EnricoDaga](../../User/EnricoDaga.md "User:EnricoDaga") says:


We can give the possibility to add references in the following way:



1. Category:WebReference
	* Property:ReferenceLabel
	* Property:ReferenceType (enumeration?)
		+ Project web site
		+ OWL/RDF ontology
		+ Others?
	* Property:ReferenceDescription
2. Then, we can give the possiblity to add references to:
	* Patterns
	* Exemplary ontologies
	* Modeling issues
	* Domains


#####  26-02-2010 [EnricoDaga](../../User/EnricoDaga.md "User:EnricoDaga") says:


The workflow ca be:



* from any page a button/link is provided 'add a reference'
* the form for a web reference is presented (the previous page is automatically setup as subject of the reference)
* the user enter data and creates the reference
* all references are automatically listed at the bottom of the page


#####  26-02-2010 [MichaelUschold](../../User/MichaelUschold.md "User:MichaelUschold") says:


This is close to what we want. I propose the following changes:



1. There should not be a distinction between a WebReference and Other reference. Instead
	1. just have one kind of reference
	2. have an optional URL field in the case of it being a web reference (e.g. called: Propery:ReferenceURL).
	3. in the case of a non-web reference, everything that is needed will be in the ReferenceDescription (e.g. a reference for a paper in a conference proceedings). Often papers have URLs too the .pdf.
2. Having OWL/RDF Ontology as a type of reference will be redundant for patterns and exemplary ontologies, and modeling issues because there already are properties for this (e.g. OWLImplemntation and OntologyURI). I'm not sure we need a type for ontology at all.
3. The types of references will therefore include:
	1. Project Home Page (instead of Project Web Site - small difference)
	2. Documentation
	3. Wiki
	4. Discussion Forum (e.g. a link to a discussion thread)
	5. Personal Communication (this may not be necessary, may not get much use)
	6. Other
4. Have a "Add Another Reference Type" button, in case there is a commonly occurring option missed.


#####  26-02-2010 [MichaelUschold](../../User/MichaelUschold.md "User:MichaelUschold") says:


I like the workflow. We may later choose to put the references somewhere else, but the bottom of the page is good for now. For example, you might want to list one or two references in the main table, and the rest below. That is a later frill.


  




#####  2-03-2010 [EnricoDaga](../../User/EnricoDaga.md "User:EnricoDaga") says:


The model is now:



* [Category:Reference](../../Category/Reference.md "Category:Reference")
	+ [Property:ReferenceSubject](../../Property/ReferenceSubject.md "Property:ReferenceSubject") (automatic, multiple)
	+ [Property:ReferenceLabel](../../Property/ReferenceLabel.md "Property:ReferenceLabel") (mandatory)
	+ [Property:ReferenceDescription](../../Property/ReferenceDescription.md "Property:ReferenceDescription") (mandatory)
	+ [Property:ReferenceURL](../../Property/ReferenceURL.md "Property:ReferenceURL") (optional)
	+ [Property:ReferenceType](../../Property/ReferenceType.md "Property:ReferenceType") (mandatory, enumeration)
		1. Project Home Page
		2. Documentation
		3. Wiki
		4. Discussion Forum
		5. Personal Communication
		6. Other
		- Have a "Add Another Reference Type" button, in case there is a commonly occurring option missed. . The list can be extended by sysop users. If the user needs a type of reference that is not in the list, he can choose 'Other' and write it in an additional field.
		- This list can be extended by editing the '[Property:ReferenceType](../../Property/ReferenceType.md "Property:ReferenceType")' page.
* References have their own page, named as follow: Community:References/<ReferenceLabel>
* Reference page shows the subject and reference data


Workflow:



* from any page a button/link is provided 'add a reference'
* The user creates a new reference. The form for a [Category:Reference](../../Category/Reference.md "Category:Reference") is presented (the previous page is automatically setup as subject of the reference)
* all references are automatically listed at the bottom of the page


__IMPORTANT: a [Category:Reference](../../Category/Reference.md "Category:Reference") is intended to represent an n-ary relation. References cannot be shared by multiple subjects!__


  






Retrieved from "[http://ontologydesignpatterns.org/wiki/Odp:Tasks/References\_for\_Exemplary\_Ontologies](../../Odp/Tasks/References_for_Exemplary_Ontologies.md)"
 [Categories](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [RootTask](../../Category/RootTask.md "Category:RootTask") | [DevelopmentTask](../../Category/DevelopmentTask.md "Category:DevelopmentTask")