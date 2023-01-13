[![](../images/thumb/b/b5/Certified.png/70px-Certified.png)](../Image/Certified.png.md "Certified.png") __This pattern has been certified.__
Related submission, with evaluation history, can be found __here__





#  Graphical representation


__Diagram__




[![Image:Parameter.jpg](../images/5/56/Parameter.jpg)](../Image/Parameter.jpg.md "Image:Parameter.jpg")




#  General description


  




#  Elements


_The __Parameter__ Content OP locally defines the following ontology elements:_



[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __hasParameter__ (owl:ObjectProperty) A Concept can have a Parameter that constrains the attributes that a classified Entity can have in a certain Situation, e.g. a 4WheelDriver Role definedIn the ItalianTrafficLaw has a MinimumAge parameter on the Amount 16. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[hasParameter](../Submissions/Parameter/hasParameter.md "Submissions:Parameter/hasParameter") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __isParameterFor__ (owl:ObjectProperty) A Concept can have a Parameter that constrains the attributes that a classified Entity can have in a certain Situation, e.g. a 4WheelDriver Role definedIn the ItalianTrafficLaw has a MinimumAge parameter on the Amount 16. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[isParameterFor](../Submissions/Parameter/isParameterFor.md "Submissions:Parameter/isParameterFor") page_
[![DatatypeProperty](../images/thumb/a/a5/DatatypeProperty.gif/20px-DatatypeProperty.gif)](../Image/DatatypeProperty.gif.md "DatatypeProperty") __hasParameterDataValue__ (owl:DatatypeProperty) Parametrizes values from a datatype. For example, a Parameter AgeForDriving hasParameterDataValue 18 on datatype xsd:int, in the Italian traffic code. In this example, AgeForDriving isDefinedIn the Norm ItalianTrafficCodeAgeDriving.
More complex parametrization requires workarounds. E.g. AgeRangeForDrugUsage could parametrize data value: 14 to 50 on the datatype: xsd:int. Since complex datatypes are not allowed in OWL1.0, a solution to this can only work by creating two 'sub-parameters': MinimumAgeRangeForDrugUsage (that hasParameterDataValue 14) and MaximumAgeRangeForDrugUsage (that hasParameterDataValue 50), which are components of the main Parameter AgeRangeForDrugUsage.


Ordering on subparameters can be created by using or specializing the object property 'precedes'. 



 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[hasParameterDataValue](../Submissions/Parameter/hasParameterDataValue.md "Submissions:Parameter/hasParameterDataValue") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif.md "Class") __Concept__ (owl:Class) A concept is a SocialObject, and isDefinedIn a Description . 
Once defined, a Concept can be used in other descriptions. 


The classifies relation relates concepts to entities at some time 



 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[Concept](../Submissions/Parameter/Concept.md "Submissions:Parameter/Concept") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif.md "Class") __Parameter__ (owl:Class) A Concept that classifies something having a certain value, e.g. 'High' can be said of people taller than 185 cm.
However, in order to formally represent this constraint, we need to add an anonymous type to a parameter instance, using a property that convey the semantics of the parameter, e.g.:


High rdf:type Person and (some hasHeight (Height and (oneOf isTallerThan 185) and (oneOf hasUnitOfMeasure centimeter))) 



 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[Parameter](../Submissions/Parameter/Parameter.md "Submissions:Parameter/Parameter") page_
#  Additional information


The parameter content ontology design pattern. This CP is extracted from the DOLCE Ultra Lite ontology. It represents parameters which are constraints or selections on observable values.



#  Scenarios



__Scenarios about Parameter__
No scenario is added to this Content OP.




#  Reviews



__Reviews about Parameter__
There is no review about this proposal.
This revision (revision ID __9108__) takes in account the reviews: none


Other info at [evaluation tab](http://ontologydesignpatterns.org/wiki/index.php?title=Submissions:Parameter&action=evaluation "http://ontologydesignpatterns.org/wiki/index.php?title=Submissions:Parameter&action=evaluation")




  




#  Modeling issues



__Modeling issues about Parameter__

  




#  References


[Add a reference](index.php@title=Odp%253AAdd_reference&subject=../Submissions/Parameter.md "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_reference&subject=Submissions%3AParameter")


  






Retrieved from "[http://ontologydesignpatterns.org/wiki/Submissions:Parameter](../Submissions/Parameter.md)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [ProposedContentOP](../Category/ProposedContentOP.md "Category:ProposedContentOP")