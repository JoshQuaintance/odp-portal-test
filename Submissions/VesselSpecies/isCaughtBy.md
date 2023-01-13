___isCaughtBy__ has [Category:OntologyElement](../../Category/OntologyElement "Category:OntologyElement") and is an [element of](../../Property/ElementOf "Property:ElementOf") [VesselSpecies](../../Submissions/VesselSpecies "Submissions:VesselSpecies")_


  




[![ObjectProperty](../../images/thumb/c/c3/ObjectProperty.gif/45px-ObjectProperty.gif)](../../Image/ObjectProperty.gif "ObjectProperty")
__Name__: isCaughtBy 


__Type:__ owl:ObjectProperty 


__Description__: Actually a composed property: this needs either a property chain, a SPARQL query, or a SWRL rule to gather a value. E.g. in SPARQL:


  



CONSTRUCT {?x :catchesSpecies ?y . ?y isCaughtBy ?x}


WHERE {


?x gearvessel:usesGearType ?z .


?z gearspecies:catchesSpecies ?y


} 





Retrieved from "[http://ontologydesignpatterns.org/wiki/Submissions:VesselSpecies/isCaughtBy](../../Submissions/GearSpecies/isCaughtBy)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [OntologyElement](../../Category/OntologyElement "Category:OntologyElement")