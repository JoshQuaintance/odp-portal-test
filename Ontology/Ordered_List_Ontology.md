Return to [Catalogue of Exemplary Ontologies](../Ontology/Main "Ontology:Main")



#  Ontology Overview


#  Long Description


There is a need to describe typed ordered lists or sequences of information resources. The existing approach in the RDF vocabulary, rdf:Seq, has some drawbacks regarding defining explicitly a range for items of a sequence and to query them efficiently with SPARQL, because every slot of a sequence is related by a separate property of the form rdf:\_N, where N is a positive integer number, e.g. rdf:\_1 (cf. RDF Vocabulary Description Language 1.0: RDF Schema and RDF Semantics ). That’s why, I co-designed the Ordered List Ontology according to a proposal made by Samer A. Abdallah. This ontology should overcome the drawbacks of the existing ordered list modelling approach by enabling more semantics to describe sequences of information resources.
As one can see in graphic 'olo:OrderedList concept as graph with relations', the Ordered List Ontology consists of two concepts - olo:OrderedList and olo:Slot. That means an ordered list is a composite of all slots, which are part of this ordered list (related by the property olo:slot). Although, the Ordered List Ontology is OWL based, the ontology also provides "backward" compatibility to the RDFS world.
The initial and primary access method to single slots in an ordered list should be olo:index, because this property represents the fixed index of a slot in an ordered list. Thereby, the property olo:length relates to the length of an ordered list, the number of included slots. The secondary access method is its (currently) optional iterator olo:next as shortcut to the next slot in the list. The items, which are arranged in an ordered list, are associated by the property olo:item to a slot.
On the basis of the ordered list concept defined in the Ordered List Ontology one can define more specific ordered list definitions, e.g. for media playlist (see the Play Back Ontology) or ranked recommendations (see the Recommendation Ontology).



#  Additional Information


  



  




#  References


[Add a reference](index.php@title=Odp%253AAdd_reference&subject=Ontology%253AOrdered+List+Ontology.html "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_reference&subject=Ontology%3AOrdered+List+Ontology")



* A blog post about the Ordered List Ontology with examples and graphics. [Weblog post](http://smiy.org/2010/07/15/the-ordered-list-ontology/ "http://smiy.org/2010/07/15/the-ordered-list-ontology/") | [reference page](../Community/References/Ordered_List_Ontology_announcement "Community:References/Ordered List Ontology announcement")




Retrieved from "[http://ontologydesignpatterns.org/wiki/Ontology:Ordered\_List\_Ontology](../Ontology/Ordered_List_Ontology)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [Ontology](../Category/Ontology "Category:Ontology")