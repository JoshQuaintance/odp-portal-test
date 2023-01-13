___hasSubEventObject__ has [Category:OntologyElement](../../Category/OntologyElement.md "Category:OntologyElement") and is an [element of](../../Property/ElementOf.md "Property:ElementOf") [EventProcessing](../../Submissions/EventProcessing.md "Submissions:EventProcessing")_


  




[![ObjectProperty](../../images/thumb/c/c3/ObjectProperty.gif/45px-ObjectProperty.gif)](../../Image/ObjectProperty.gif.md "ObjectProperty")
__Name__: hasSubEventObject 


__Type:__ owl:TransitiveProperty 


__Description__: A relation that connects a complex event with the low-level events it is a higher-level representation of. An event object may reference another event, on a lower level of abstraction or granularity, upon which is it is based or from which it was derived or triggered, making that other event a "sub event" of this aggregated or more abstract event object. Note that for modelling instance data, normally, the non-transitive sub-property "hasDirectSubEventObject" should be used, based on which the presence of this transitive relation can be inferred. 





Retrieved from "[http://ontologydesignpatterns.org/wiki/Submissions:EventProcessing/hasSubEventObject](../../Submissions/EventProcessing/hasSubEventObject.md)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [OntologyElement](../../Category/OntologyElement.md "Category:OntologyElement")