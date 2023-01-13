[![](../images/thumb/b/b5/Certified.png/70px-Certified.png)](../Image/Certified.png "Certified.png") __This pattern has been certified.__
Related submission, with evaluation history, can be found __here__






[![Image:Vesselspecies.jpg](http://ontologydesignpatterns.org/wiki/images/8/84/Vesselspecies.jpg)](http://ontologydesignpatterns.org/wiki/Image:Vesselspecies.jpg "Image:Vesselspecies.jpg")




#  General description


  




#  Elements


_The __VesselSpecies__ Content OP locally defines the following ontology elements:_



[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif "Class") __AquaticSpecies__ (owl:Class) Aquatic species are conceptual entities that are characterized together with resources and water areas. 
Mappable to fi:Species, fi:SpeciesRef, fi:SpeciesFeature, etc.


It has related axioms from FIGIS Schema that are included in the classes linked to the fi:Species class, such as fi:SpeciesRef (holding association with fi:AqResRef, which holds association with fi:WaterAreaRef). 



 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[AquaticSpecies](http://ontologydesignpatterns.org/wiki/Submissions:VesselSpecies/AquaticSpecies "Submissions:VesselSpecies/AquaticSpecies") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif "Class") __VesselType__ (owl:Class) Vessel types are conceptual entities. 
Mappable to fi:VesseltypeRef 



 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[VesselType](http://ontologydesignpatterns.org/wiki/Submissions:VesselSpecies/VesselType "Submissions:VesselSpecies/VesselType") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif "ObjectProperty") __catchesSpecies__ (owl:ObjectProperty) Actually a composed property: this needs either a property chain, a SPARQL query, or a SWRL rule to gather a value. E.g. in SPARQL:
  



CONSTRUCT {?x :catchesSpecies ?y . ?y isCaughtBy ?x}


WHERE {


?x gearvessel:usesGearType ?z .


?z gearspecies:catchesSpecies ?y


} 



 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[catchesSpecies](../Submissions/VesselSpecies/catchesSpecies "Submissions:VesselSpecies/catchesSpecies") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif "ObjectProperty") __isCaughtBy__ (owl:ObjectProperty) Actually a composed property: this needs either a property chain, a SPARQL query, or a SWRL rule to gather a value. E.g. in SPARQL:
  



CONSTRUCT {?x :catchesSpecies ?y . ?y isCaughtBy ?x}


WHERE {


?x gearvessel:usesGearType ?z .


?z gearspecies:catchesSpecies ?y


} 



 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[isCaughtBy](../Submissions/VesselSpecies/isCaughtBy "Submissions:VesselSpecies/isCaughtBy") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif "ObjectProperty") __isCaughtByVesselType__ (owl:ObjectProperty) 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[isCaughtByVesselType](../Submissions/VesselSpecies/isCaughtByVesselType "Submissions:VesselSpecies/isCaughtByVesselType") page_
(type): [http://www.w3.org/2002/07/owl#Ontology](http://www.w3.org/2002/07/owl#Ontology "http://www.w3.org/2002/07/owl#Ontology")


(relatedCPs): [http://www.ontologydesignpatterns.org/cp/owl/fsdas/gearspecies.owl](http://www.ontologydesignpatterns.org/cp/owl/fsdas/gearspecies.owl "http://www.ontologydesignpatterns.org/cp/owl/fsdas/gearspecies.owl")


(imports): [http://www.ontologydesignpatterns.org/schemas/cpannotationschema.owl](http://www.ontologydesignpatterns.org/schemas/cpannotationschema.owl "http://www.ontologydesignpatterns.org/schemas/cpannotationschema.owl")


(versionInfo): Created by Alessandro Adamou


(versionInfo): 1.0



#  Scenarios



__Scenarios about VesselSpecies__
No scenario is added to this Content OP.




#  Reviews



__Reviews about VesselSpecies__
This revision (revision ID __3686__) takes in account the reviews: [AldoGangemi about VesselSpecies](../Reviews/AldoGangemi_about_VesselSpecies "Reviews:AldoGangemi about VesselSpecies")


Other info at [evaluation tab](http://ontologydesignpatterns.org/wiki/index.php?title=Submissions:VesselSpecies&action=evaluation "http://ontologydesignpatterns.org/wiki/index.php?title=Submissions:VesselSpecies&action=evaluation")






Retrieved from "[http://ontologydesignpatterns.org/wiki/Submissions:VesselSpecies](../Submissions/VesselSpecies)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [ProposedContentOP](../Category/ProposedContentOP "Category:ProposedContentOP")