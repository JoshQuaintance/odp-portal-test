[![](../images/thumb/b/b5/Certified.png/70px-Certified.png)](../Image/Certified.png.md "Certified.png") __This pattern has been certified.__
Related submission, with evaluation history, can be found __here__





#  Graphical representation


__Diagram__




[![Image:Speciesnames.jpg](../images/3/32/Speciesnames.jpg)](../Image/Speciesnames.jpg.md "Image:Speciesnames.jpg")




#  General description


  




#  Elements


_The __SpeciesNames__ Content OP locally defines the following ontology elements:_



[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif.md "Class") __AquaticSpecies__ (owl:Class) Aquatic species are conceptual entities that are characterized together with resources and water areas. 
Mappable to fi:Species, fi:SpeciesRef, fi:SpeciesFeature, etc.


It has related axioms from FIGIS Schema that are included in the classes linked to the fi:Species class, such as fi:SpeciesRef (holding association with fi:AqResRef, which holds association with fi:WaterAreaRef). 



 [![](../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[AquaticSpecies](../Submissions/SpeciesNames/AquaticSpecies.md "Submissions:SpeciesNames/AquaticSpecies") page_
[![DatatypeProperty](../../../images/thumb/a/a5/DatatypeProperty.gif/20px-DatatypeProperty.gif)](../Image/DatatypeProperty.gif.md "DatatypeProperty") __hasLocalName__ (owl:DatatypeProperty) Property to express a species' localname , where it is used , and any additional information like the name of the dialect or more detailed geographical information on where exactly the local-common name is used for the aquatic species in a given country. 
 [![](../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[hasLocalName](../Submissions/SpeciesNames/hasLocalName.md "Submissions:SpeciesNames/hasLocalName") page_
[![DatatypeProperty](../../../images/thumb/a/a5/DatatypeProperty.gif/20px-DatatypeProperty.gif)](../Image/DatatypeProperty.gif.md "DatatypeProperty") __canBeConfusedWith__ (owl:DatatypeProperty) A property for expressing a description of why a species may be confused with another. It may instead/also contain a list of other species with which a species may be confused. 
 [![](../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[canBeConfusedWith](../Submissions/SpeciesNames/canBeConfusedWith.md "Submissions:SpeciesNames/canBeConfusedWith") page_
[![DatatypeProperty](../../../images/thumb/a/a5/DatatypeProperty.gif/20px-DatatypeProperty.gif)](../Image/DatatypeProperty.gif.md "DatatypeProperty") __hasSynonym__ (owl:DatatypeProperty) Expresses the scientific names that exist for a species but are no longer valid. 
 [![](../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[hasSynonym](../Submissions/SpeciesNames/hasSynonym.md "Submissions:SpeciesNames/hasSynonym") page_
#  Additional information


(type): [http://www.w3.org/2002/07/owl#Ontology](http://www.w3.org/2002/07/owl#Ontology "http://www.w3.org/2002/07/owl#Ontology")


(imports): [http://www.ontologydesignpatterns.org/schemas/cpannotationschema.owl](http://www.ontologydesignpatterns.org/schemas/cpannotationschema.owl "http://www.ontologydesignpatterns.org/schemas/cpannotationschema.owl")


(versionInfo): 1.0



#  Scenarios



__Scenarios about SpeciesNames__
No scenario is added to this Content OP.




#  Reviews



__Reviews about SpeciesNames__
There is no review about this proposal.
This revision (revision ID __9128__) takes in account the reviews: none


Other info at [evaluation tab](http://ontologydesignpatterns.org/wiki/index.php?title=Submissions:SpeciesNames&action=evaluation "http://ontologydesignpatterns.org/wiki/index.php?title=Submissions:SpeciesNames&action=evaluation")




  




#  Modeling issues



__Modeling issues about SpeciesNames__
There is no Modeling issue related to this proposal.




  




#  References


[Add a reference](index.php@title=Odp%253AAdd_reference&subject=../Submissions/SpeciesNames.md "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_reference&subject=Submissions%3ASpeciesNames")


  






Retrieved from "[http://ontologydesignpatterns.org/wiki/Submissions:SpeciesNames](../Submissions/SpeciesNames.md)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [ProposedContentOP](../Category/ProposedContentOP.md "Category:ProposedContentOP")