Return to [Catalogue of Exemplary Ontologies](../Ontology/Main "Ontology:Main")



#  Ontology Overview


#  Long Description


It seems that there is still a lack in modelling contextual information for Semantic Graph triples and deploying this knowledge representation reusable in a distributed Linked Data environment. Although, there exists probably applicable solutions for representing external context\*, e.g. Named Graphs or N-Quads. However, these methods are not really appropriated to represent internal context\* by keeping clear semantics regarding their described Semantic Graph triples (information resource). Even the existing method for RDF statements, RDF Reification (statement reification), has no clear semantics between the statement triple(s) and their reification information resource(s). Furthermore, this method is intended to be applied at the instance level. Although, it might be good to be able to apply reification definition also on the vocabulary level. That means, to reify the semantic relation that is established by a property. This kind of reification is then called property reification.
Therefore, the simple semantic relation, represented by subject, predicate and object, is now defined as shortcut relation. Thereby, the predicate is always the same property for a single shortcut relation definition. Beyond, the class that enables a detailed description of such a n-ary relation is called reification class.
Due to the reason, that there wasn’t a published vocabulary that addresses a mapping and its semantics between shortcut relations and reification classes and vice versa, Bob Ferris co-designed the Property Reification Vocabulary. This vocabulary is designed after a proposal made by Jiří Procházka, Richard Cyganiak and Toby Inkster and was also extended by Bob Ferris to enable further functionality. It should reflect the important use case and ontology design pattern of property reification. This gives ontology designers the freedom to separate such property reification definitions from their core ontology definition and enable hence the opportunity to make them optional.



#  Additional Information


  



  




#  References


[Add a reference](index.php@title=Odp%253AAdd_reference&subject=Ontology%253AProperty+Reification+Vocabulary.html "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_reference&subject=Ontology%3AProperty+Reification+Vocabulary")



* The working page of the Property Reification Vocabulary on the ESW wiki. [Wiki](http://esw.w3.org/PropertyReificationVocabulary "http://esw.w3.org/PropertyReificationVocabulary") | [reference page](../Community/References/Property_Reification_RDF_Vocabulary "Community:References/Property Reification RDF Vocabulary")




Retrieved from "[http://ontologydesignpatterns.org/wiki/Ontology:Property\_Reification\_Vocabulary](../Ontology/Property_Reification_Vocabulary)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [Ontology](../Category/Ontology "Category:Ontology")