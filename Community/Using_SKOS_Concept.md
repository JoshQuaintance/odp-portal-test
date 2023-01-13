#  Using SKOS Concept


__Title:__ General Issue: Using SKOS Concept


__Description:__ General Issue: When should something be an instance of SKOS:Concept? 


__Diagram__
_(this article has no graphical representation)_



#  About


  




#  Additional information


_Issue_: When should something be an instance of SKOS:Concept?


_Source_: [W3C Linked Open Data discussion list](http://lists.w3.org/Archives/Public/public-lod/ "http://lists.w3.org/Archives/Public/public-lod/")


_Related Discussions:_ [Using DBpedia resources as skos:Concepts](http://markmail.org/message/hgnfj4uimr4mx7yx "http://markmail.org/message/hgnfj4uimr4mx7yx")


_Related Modeling Issues_: [Representing Species](../Community/Representing_Species "Community:Representing Species")


_Example_: [Does it make sense to have an individual cougar be an instance of SKOS:Concept?](http://lists.w3.org/Archives/Public/public-lod/2009Dec/0034.html "http://lists.w3.org/Archives/Public/public-lod/2009Dec/0034.html")


_Conclusions_: 



1. a class of things (e.g. animals) is naturally represented as a a SKOS:Concept
2. it is not natural to represent individuals, e.g. a particular cougar, as a SKOS:Concept
3. The SKOS documentation leaves a lot of latitude for interpreting the meaning of SKOS:Concept, especially with respect to how it relates to OWL and RDF modeling.
4. It is much easier to map any given ontology onto a knowledge organize system than going the other way.


  

Definition from SKOS documentation:


The class skos:Concept is the class of SKOS concepts.


A SKOS concept can be viewed as an idea or notion; a unit of thought. However, what constitutes a "unit of thought" is subjective, and this definition is meant to be suggestive, rather than restrictive. 


The notion of a SKOS concept is useful when describing the conceptual or intellectual structure of a knowledge organization system, and when referring to specific ideas or meanings established within a KOS.


Note that, because SKOS is designed to be a vehicle for representing semi-formal KOS, such as thesauri and classification schemes, a certain amount of flexibility has been built in to the formal definition of this class.


See the [SKOS Primer](http://www.w3.org/TR/skos-primer "http://www.w3.org/TR/skos-primer") for more examples of identifying and describing SKOS concepts.


  

Here is what the SKOS Primer says:


The fundamental element of the SKOS vocabulary is the concept. Concepts are the units of thought, ideas, meanings, or (categories of) objects and events - which underlie many knowledge organization systems. As such, concepts exist in the mind as abstract entities which are independent of the terms used to label them.


<snip>


For example (in Turtle notation):




```
ex:animals rdf:type skos:Concept.

```

So, one criteria might be: Can the thing be conceived as part of a knowledge organization system? It is easier to answer yes to this question for a class like Cougar than for an instance of a class, an individual cougar. However, this gives rise to the question of modeling classes as instances, which is problematic in OWL-DL. (See related modelling issue [[Community:GI Representing Species]]).


  

It may be safer to use a class as a concept than vice versa. One person [noted that](http://lists.w3.org/Archives/Public/public-lod/2009Dec/0044.html "http://lists.w3.org/Archives/Public/public-lod/2009Dec/0044.html"): “All (RDFS/OWL) ontologies can be regarded as knowledge organization systems, but KOSs are generally not trivially mapped into ontologies.”


  

The [SKOS reference](http://www.w3.org/TR/2009/CR-skos-reference-20090317/#concepts "http://www.w3.org/TR/2009/CR-skos-reference-20090317/#concepts") explicitly says there is no commitment about the relationship between SKOS:Concepts and OWL:Classes and OWL:Properties. User may explore different models for this. So Cougar can be both a skos:Concept and an owl:Class. Or it could be both a skos:Concept and an owl:ObjectProperty. 


  

One [good comment](http://www.mail-archive.com/public-lod@w3.org/msg04031.html "http://www.mail-archive.com/public-lod@w3.org/msg04031.html") is that: 


the link between a document and its subject should be represented by a dedicated property that is not rdf:type. If people generally adopted this pattern, there would be less chance of someone's using the cougar concept as the class of documents about cougars, which I expect is the most likely confusion.


  

DBpedia uses the property skos:Subject to relate Wikipedia articles to their categories. [Leigh Dodds contributes](http://lists.w3.org/Archives/Public/public-lod/2009Dec/0145.html "http://lists.w3.org/Archives/Public/public-lod/2009Dec/0145.html"): I did some digging around and found that



* Dbpedia and Uniprot model taxa as instances, as does the RDF data coming from the Ubio LSID resolver
* The ETHAN ontology, and the TWDG TaxonConcept model (AIUI), both model taxa as Classes
* Peter's species concept examples use skos:Concepts which are themselves instances rather than classes.
* OpenCyc uses Collections which seem to be a little of both :)


  

The discussion seems to be missing the fact that in rdf, you can do whatever you want. Competency questions have not entered the discussion. They should be the guide to determine what reasoning requirements they have. Without a focus on clear requirements, the discussion participants are to some extent, wandering around in the dark.


There was one exception to this. [Peter Devries contributes](http://lists.w3.org/Archives/Public/public-lod/2009Dec/0147.html%20 "http://lists.w3.org/Archives/Public/public-lod/2009Dec/0147.html%20"): 


It looks to me as if TDWG really wants to model species as a fully phylogenetic representation, but ecologists and epidemiologists need a representation that separates the idea that there is a species from the idea that that species is it's current ephemeral phylogenetic hypothesis.


Maybe someone of the list has some ideas as to which representations are best for these different use cases.



#  References


[Add a reference](index.php@title=Odp%253AAdd_reference&subject=Community%253AUsing+SKOS+Concept.html "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_reference&subject=Community%3AUsing+SKOS+Concept")


  




 [List of Modeling Issues](../Community/Main "Community:Main") | [Post a new modeling issue](../Community/PostModelingIssue "Community:PostModelingIssue") | [Add a comment in the discussion page](index.php@title=Odp%253AAdd_comment&target=Community_talk%253AUsing_SKOS_Concept.html#New_comment "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_comment&target=Community_talk:Using_SKOS_Concept#New_comment")


Retrieved from "[http://ontologydesignpatterns.org/wiki/Community:Using\_SKOS\_Concept](../Community/Using_SKOS_Concept)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [ModelingIssue](../Category/ModelingIssue "Category:ModelingIssue")