[![](../images/thumb/b/b5/Certified.png/70px-Certified.png)](../Image/Certified.png "Certified.png") __This pattern has been certified.__
Related submission, with evaluation history, can be found __here__





#  Graphical representation


__Diagram__
_(this article has no graphical representation)_



#  General description


  




#  Elements


_The __ClimaticZone__ Content OP locally defines the following ontology elements:_



[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif "Class") __ClimaticZone__ (owl:Class) 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[ClimaticZone](../Submissions/ClimaticZone/ClimaticZone "Submissions:ClimaticZone/ClimaticZone") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif "Class") __AquaticResource__ (owl:Class) A fishery resource (a collection of actual aquatic organisms) that can include aquatic organisms from different AquaticSpecies, and is localized in some WaterArea.
It can be mapped to fi:AqResRef 



 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[AquaticResource](../Submissions/ClimaticZone/AquaticResource "Submissions:ClimaticZone/AquaticResource") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif "Class") __AquaticResourceObservation__ (owl:Class) An observation of a resource characterised by different parameters. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[AquaticResourceObservation](../Submissions/ClimaticZone/AquaticResourceObservation "Submissions:ClimaticZone/AquaticResourceObservation") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif "ObjectProperty") __hasResource__ (owl:ObjectProperty) 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[hasResource](../Submissions/ClimaticZone/hasResource "Submissions:ClimaticZone/hasResource") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif "ObjectProperty") __hasClimaticZone__ (owl:ObjectProperty) 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[hasClimaticZone](../Submissions/ClimaticZone/hasClimaticZone "Submissions:ClimaticZone/hasClimaticZone") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif "ObjectProperty") __isClimaticZoneOf__ (owl:ObjectProperty) 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[isClimaticZoneOf](../Submissions/ClimaticZone/isClimaticZoneOf "Submissions:ClimaticZone/isClimaticZoneOf") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif "ObjectProperty") __isResourceOf__ (owl:ObjectProperty) 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[isResourceOf](../Submissions/ClimaticZone/isResourceOf "Submissions:ClimaticZone/isResourceOf") page_
[![DatatypeProperty](../images/thumb/a/a5/DatatypeProperty.gif/20px-DatatypeProperty.gif)](../Image/DatatypeProperty.gif "DatatypeProperty") __hasReferenceYear__ (owl:DatatypeProperty) 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[hasReferenceYear](../Submissions/ClimaticZone/hasReferenceYear "Submissions:ClimaticZone/hasReferenceYear") page_
#  Additional information


(type): [http://www.w3.org/2002/07/owl#Ontology](http://www.w3.org/2002/07/owl#Ontology "http://www.w3.org/2002/07/owl#Ontology")


(imports): [http://www.ontologydesignpatterns.org/cp/owl/observation.owl](http://www.ontologydesignpatterns.org/cp/owl/observation.owl "http://www.ontologydesignpatterns.org/cp/owl/observation.owl")


(imports): [http://www.ontologydesignpatterns.org/cp/owl/fsdas/aquaticresources.owl](http://www.ontologydesignpatterns.org/cp/owl/fsdas/aquaticresources.owl "http://www.ontologydesignpatterns.org/cp/owl/fsdas/aquaticresources.owl")


(versionInfo): Created by Eva Blomqvist


(hasUnitTest): SELECT ?x WHERE {?x a :AquaticResourceObservation.  ?x :hasClimaticZone :Tropical}


(versionInfo): 1.0


(imports): [http://www.ontologydesignpatterns.org/schemas/cpannotationschema.owl](http://www.ontologydesignpatterns.org/schemas/cpannotationschema.owl "http://www.ontologydesignpatterns.org/schemas/cpannotationschema.owl")



#  Scenarios



__Scenarios about ClimaticZone__
No scenario is added to this Content OP.




#  Reviews



__Reviews about ClimaticZone__
There is no review about this proposal.
This revision (revision ID __8837__) takes in account the reviews: none


Other info at [evaluation tab](http://ontologydesignpatterns.org/wiki/index.php?title=Submissions:ClimaticZone&action=evaluation "http://ontologydesignpatterns.org/wiki/index.php?title=Submissions:ClimaticZone&action=evaluation")




  




#  Modeling issues



__Modeling issues about ClimaticZone__
There is no Modeling issue related to this proposal.




  




#  References


[Add a reference](index.php@title=Odp%253AAdd_reference&subject=../Submissions/ClimaticZone "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_reference&subject=Submissions%3AClimaticZone")


  






Retrieved from "[http://ontologydesignpatterns.org/wiki/Submissions:ClimaticZone](../Submissions/ClimaticZone)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [ProposedContentOP](../Category/ProposedContentOP "Category:ProposedContentOP")