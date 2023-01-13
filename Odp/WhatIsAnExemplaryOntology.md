* [Visit the catalogue of Exemplary Ontologies](../Ontology/Main.md "Ontology:Main")
* [Exemplary Ontologies FAQ](../Odp/Exemplary_ontology_FAQ.md "Odp:Exemplary ontology FAQ")


##  What is an Exemplary Ontology?


An exemplary ontology is one that can serve as a model that can be imitated or leveraged by ontology engineers in the future. The most fundamental property of an exemplary ontology is being _well designed for its intended purpose_. Think of a paper clip - from a purely utilitarian perspective, it went through many stages of evolution before it became a thing of elegant simplicity - linked to a specific purpose. From a design perspective it is a thing of beauty. Nothing is extraneous, it just works. So it is with any well designed artifact. Any ontology that has reached a similar pinnacle of good design will have many of the following properties:



1. well designed for its purpose.
2. explicitly stated requirements (especially competency questions) were specified and used to guide the design process.
3. meets _all_ and for the most part, _only_ the intended requirements;
4. does not make unnecessary commitments or assumptions
5. will be easy to extend to meet additional unknown future requirements
6. it reuses as much as possible
	1. leverages upper level ontologies where appropriate
	2. leverages existing domain ontologies
	3. instantiates known design patterns
7. there is a core set of primitives that are used to build up more complex parts. This is a kind of reuse within the same ontology, as opposed to reusing external ontologies and patterns. The coralary to this is: the same concepts are not created independently multiple times in different places in the ontology.
8. easy to understand and maintain;
	1. avoids hacks and workarounds (which tend to be ugly anyway)
	2. lacks redundancy (related to point about reusing primitives)
9. well documented
	1. describes the core ideas of the ontology
	2. describes the core classes and relationships
	3. includes diagrams to illustrate 1&2 above


The reason for the ontology meeting _only_ the intended requirements is to keep the ontology as lean as possible. The ontology should of course contain things that help ensure that it can easily expanded to meet as yet unanticipated future requirements -- even if they are not strictly needed to meet stated requirements.





Retrieved from "[http://ontologydesignpatterns.org/wiki/Odp:WhatIsAnExemplaryOntology](../Odp/WhatIsAnExemplaryOntology.md)"