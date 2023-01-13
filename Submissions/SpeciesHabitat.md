[![](../images/thumb/b/b5/Certified.png/70px-Certified.png)](../Image/Certified.png.md "Certified.png") __This pattern has been certified.__
Related submission, with evaluation history, can be found __here__





#  Graphical representation


__Diagram__




[![Image:Specieshabitat.jpg](../images/6/63/Specieshabitat.jpg)](../Image/Specieshabitat.jpg.md "Image:Specieshabitat.jpg")




#  General description


  




#  Elements


_The __SpeciesHabitat__ Content OP locally defines the following ontology elements:_



[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif.md "Class") __Habitat__ (owl:Class) Habitat is the biological and ecological context of a species in the area of an aquatic resource. 
 [![](../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[Habitat](../Submissions/SpeciesHabitat/Habitat.md "Submissions:SpeciesHabitat/Habitat") page_
[![ObjectProperty](../../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __hasHabitat__ (owl:ObjectProperty) 
 [![](../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[hasHabitat](../Submissions/SpeciesHabitat/hasHabitat.md "Submissions:SpeciesHabitat/hasHabitat") page_
[![ObjectProperty](../../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __isHabitatFor__ (owl:ObjectProperty) 
 [![](../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[isHabitatFor](../Submissions/SpeciesHabitat/isHabitatFor.md "Submissions:SpeciesHabitat/isHabitatFor") page_
#  Additional information


This pattern encodes a FSDAS competency question, with an indication to use some Species class, and some hasHabitat property, with range xsd:string.
Since the application task of FSDAS is to jointly query FIGIS factsheet data and RTMS time series data, the pattern must encode elements that can be easily mapped to FIGIS and RTMS schemas/ontologies.
Issue (1) mapping Species to FIGIS schema, since the needed schema elements are two instead of one.
Issue (2) representation of habitats in the pattern is intuitively with objects, since habitats are typically objects, and points in a value space (as the referents of xsd datatypes typically are). The suggestion in the competencey question is to use xsd.string though.


(type): [http://www.w3.org/2002/07/owl#Ontology](http://www.w3.org/2002/07/owl#Ontology "http://www.w3.org/2002/07/owl#Ontology")


(versionInfo): Created by Aldo Gangemi


(imports): [http://www.ontologydesignpatterns.org/cp/owl/fsdas/aquaticresources.owl](http://www.ontologydesignpatterns.org/cp/owl/fsdas/aquaticresources.owl "http://www.ontologydesignpatterns.org/cp/owl/fsdas/aquaticresources.owl")


(versionInfo): 1.0


(imports): [http://www.ontologydesignpatterns.org/schemas/cpannotationschema.owl](http://www.ontologydesignpatterns.org/schemas/cpannotationschema.owl "http://www.ontologydesignpatterns.org/schemas/cpannotationschema.owl")


(comment): This pattern encodes a FSDAS competency question, with an indication to use some Species class, and some hasHabitat property, with range xsd:string.
Since the application task of FSDAS is to jointly query FIGIS factsheet data and RTMS time series data, the pattern must encode elements that can be easily mapped to FIGIS and RTMS schemas/ontologies.
Issue (1) mapping Species to FIGIS schema, since the needed schema elements are two instead of one.
Issue (2) representation of habitats in the pattern is intuitively with objects, since habitats are typically objects, and points in a value space (as the referents of xsd datatypes typically are). The suggestion in the competencey question is to use xsd.string though.



#  Scenarios



__Scenarios about SpeciesHabitat__
No scenario is added to this Content OP.




#  Reviews



__Reviews about SpeciesHabitat__
There is no review about this proposal.
This revision (revision ID __9127__) takes in account the reviews: none


Other info at [evaluation tab](http://ontologydesignpatterns.org/wiki/index.php?title=Submissions:SpeciesHabitat&action=evaluation "http://ontologydesignpatterns.org/wiki/index.php?title=Submissions:SpeciesHabitat&action=evaluation")




  




#  Modeling issues



__Modeling issues about SpeciesHabitat__
There is no Modeling issue related to this proposal.




  




#  References


[Add a reference](index.php@title=Odp%253AAdd_reference&subject=../Submissions/SpeciesHabitat.md "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_reference&subject=Submissions%3ASpeciesHabitat")


  






Retrieved from "[http://ontologydesignpatterns.org/wiki/Submissions:SpeciesHabitat](../Submissions/SpeciesHabitat.md)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [ProposedContentOP](../Category/ProposedContentOP.md "Category:ProposedContentOP")