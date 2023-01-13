#  Representing Species


__Title:__ General Issue: Representing Species


__Description:__ How should species be represented? 


__Diagram__
_(this article has no graphical representation)_



#  About


  




#  Additional information


_Issue_: What is the best way to represent species?


_Source:_ [W3C Linked Open Data discussion list](http://lists.w3.org/Archives/Public/public-lod/ "http://lists.w3.org/Archives/Public/public-lod/")


_Related Discussions:_



* [Species Concept Mapping RDF fixes and question, should the species be represented as a class?](http://lists.w3.org/Archives/Public/public-lod/2009Dec/0015.html "http://lists.w3.org/Archives/Public/public-lod/2009Dec/0015.html")
* [Lightweight RDF to Map Various Semantic Representations of Species](http://lists.w3.org/Archives/Public/public-lod/2009Nov/0176.html "http://lists.w3.org/Archives/Public/public-lod/2009Nov/0176.html")


_Related Modeling Issues:_ [Using SKOS Concept](../Community/Using_SKOS_Concept.md "Community:Using SKOS Concept")


_Example:_ There is a requirement to represent large number of species for the purpose of indexing research papers and experiments that use or refer to a species in some way.


_Conclusions:_



1. There is no one right answer, it depends on your needs.
	1. Some projects represent species as instances (e.g. DBpedia and Uniprot),
	2. Some projects represent them as classes - _e.g._ the ETHAN ontology, and the TWDG TaxonConcept model (AIUI).
	3. There are literally millions of species. Representing large numbers of them as classes may not scale.
	4. If you need to reason about the properties that define a species, and if you want to classify individuals according to their properties, you probably want to represent the species as classes.
2. If you think of species as classes, but you also want to use particular species as values of properties, then look at the document: [Representing Classes As Property Values on the Semantic Web](http://www.w3.org/TR/swbp-classes-as-values/ "http://www.w3.org/TR/swbp-classes-as-values/") for an in depth analysis of the pros and cons of various approaches.
3. You can try to have it both ways:


1. It may be possible to have two or more representations simultaneously, if you are careful.
2. OWL2 punning alows you can represent a species both as a class and as an instance. Caveat: some extra work is needed because statements about e.g. Cougar the instance will not automatically hold for statements about Cougar the class.
3. It may be possible to translate between different representations to map data or access other knowledge bases and ontologies.


1. To decide what your need are, identify your requirements, capture them as a set of competency questions and design the ontology accordingly.


___General Discussion_:__


There are different ways to view and use the idea of a species. Below are three. The first is useful for dealing with taxonomy evolution, the second is useful for dealing with observations, e.g. in Wisconsin. The third is useful for library classification.



1. A species, e.g. Homo Sapien, is represented as an instance of a class: Species
2. A species is represented as a Class whose instances are individual plants or animals of the given species. Individual species would be subclasses of e.g. Plant or Animal.
3. A species is represented as a skos:Concept


_Having multiple representations_.


OWL 2 punning was discussed by Pat Hayes. It allows for, e.g. Cougar to exist both as a class and as an instance. However, as described in [http://www.w3.org/TR/2009/REC-owl2-syntax-20091027/#Metamodeling](http://www.w3.org/TR/2009/REC-owl2-syntax-20091027/#Metamodeling "http://www.w3.org/TR/2009/REC-owl2-syntax-20091027/#Metamodeling"), when a resource is mentioned as both an individual and a class, the two mentions are interpreted independently. Axioms about the instance do not apply to the class, and vice versa. Extra work would be needed to ensure that the semantics of each was identical. Owl 2 style punning allows A sameAs B when considered as individuals but not A sameClassAs B as classes. So you have to go to the trouble of asserting the appropriate identity (possibly twice). This way, everything can work out as it should.


Bernard Vatant describes how multiple representations can virtuall co-exist by mapping from one to the other in rules. This is explained [in this post](http://lists.w3.org/Archives/Public/public-lod/2009Dec/0069.html "http://lists.w3.org/Archives/Public/public-lod/2009Dec/0069.html"). The basic idea is to us the 'construct' construct in SPARQL. Below is a portion quoted directly:


  

Suppose I have an ontology O1 where species are rept as instances of owl:Class, and an ontology O2 where species are represented as instances of skos:Concept. O1 and O2 leverage the same reference code, say ITIS. In O1 ITIS code is a datatype property o1:ITISCode which can be attached to any individual living creature, and a species class can be defined by containing all individuals sharing a given code, e.g.,


  

o1:FelisConcolor a owl:Class


owl:equivalentClass




```
  [owl:Restriction
    owl:onProperty  o1:ITISCode
    owl:hasvalue  '552479' ]

```

In O2 each concept is identified by the code using e.g., a subproperty of


skos:notation, say o2:ITISCode


  

o2:FelisConcolor a skos:Concept


o2:FelisConcolor o2:ITISCode '552479'


  

Note that sharing a code value is enough for mapping those two representations, for all pragmatic purpose. I can rely on SPARQL to find all concepts in O2 translating a class in O1 by the following request on the merged graph O1 U O2


  

SELECT ?cl ?co




```
WHERE  [?cl owl:equivalentClass  ?r.
        ?r a owl:Restriction.
        ?r  owl:onProperty   o1:ITIScode.
        ?r  owl:hasValue   ?n.
        ?co   a  skos:Concept.
        ?co   o2:ITISCode  ?n.
        ]

```

Suppose now you want to translate a class subsumption in O1 into a broader-narrower (transitive) hierarchy in O2. There yo can use a SPARQL CONSTRUCT


  

CONSTRUCT [?co1 skos:broaderTransitive ?co2]


  

WHERE [




```
              ?cl1 owl:equivalentClass  ?r1.
              ?r1 a owl:Restriction.
              ?r1  owl:onProperty   o1:ITIScode.
              ?r1  owl:hasValue   ?n1.
              ?co1   a  skos:Concept.
              ?co1   o2:ITISCode  ?n1.

```


```
              ?cl2 owl:equivalentClass  ?r2.
              ?r2 a owl:Restriction.
              ?r2  owl:onProperty   o1:ITIScode.
              ?r2  owl:hasValue   ?n2.
              ?co2   a  skos:Concept.
              ?co2   o2:ITISCode  ?n2.

```


```
              ?cl1   rdfs:subClassOf   ?cl2.
              ]

```

This marks the end of Benard Vatant's contribution. Finally, Peter DeVries described an alternative approach including encoded examples in RDF and OWL [in this post](http://lists.w3.org/Archives/Public/public-lod/2009Dec/0049.html "http://lists.w3.org/Archives/Public/public-lod/2009Dec/0049.html"). He offered the following summary of the discussion: 


I guess the issue can be summed up in the following way:



* Can you create a lightweight representation of a species that contains what most people need, but still retains the ability to link to a more complete representation for those who may need to determine the attributes and properties that are used to separate one species concept from another?
* This more complete species document, in OWL or RDF, would help determine which species concept is the best match for a given specimen?
* A species is a sort of conceptualization and it is not always obvious or generally accepted where the clear boundary between two species is.
* I think it is possible to create documents that clear up what is meant by a specific species identifier.
* This will not end the discussion of what a species is, but it will make it possible to determine if a particular specimen is a close match to the concept as it is defined.


For those interested, I have new versions of these:



* RDF Example [http://rdf.taxonconcept.org/ses/v6n7p.rdf](http://rdf.taxonconcept.org/ses/v6n7p.rdf "http://rdf.taxonconcept.org/ses/v6n7p.rdf")
* Ontology [http://rdf.taxonconcept.org/ont/txn.owl](http://rdf.taxonconcept.org/ont/txn.owl "http://rdf.taxonconcept.org/ont/txn.owl")
* Ontology Doc: [http://rdf.taxonconcept.org/ont/txn\_doc/index.html](http://rdf.taxonconcept.org/ont/txn_doc/index.html "http://rdf.taxonconcept.org/ont/txn_doc/index.html")


I also made an example RDF that tags various webpages to that species concept: [http://rdf.taxonconcept.org/webpages/v6n7p.rdf](http://rdf.taxonconcept.org/webpages/v6n7p.rdf "http://rdf.taxonconcept.org/webpages/v6n7p.rdf")


All these example RDF and OWL files are combined into one RDF file that can be used to see how they fit together: [http://rdf.taxonconcept.org/taxonconcept.rdf](http://rdf.taxonconcept.org/taxonconcept.rdf "http://rdf.taxonconcept.org/taxonconcept.rdf")



#  References


[Add a reference](index.php@title=Odp%253AAdd_reference&subject=Community%253ARepresenting+Species.html "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_reference&subject=Community%3ARepresenting+Species")


  




 [List of Modeling Issues](../Community/Main.md "Community:Main") | [Post a new modeling issue](../Community/PostModelingIssue.md "Community:PostModelingIssue") | [Add a comment in the discussion page](index.php@title=Odp%253AAdd_comment&target=Community_talk%253ARepresenting_Species.html#New_comment "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_comment&target=Community_talk:Representing_Species#New_comment")


Retrieved from "[http://ontologydesignpatterns.org/wiki/Community:Representing\_Species](../Community/Representing_Species.md)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [ModelingIssue](../Category/ModelingIssue.md "Category:ModelingIssue")