[![](../images/thumb/b/b5/Certified.png/70px-Certified.png)](../Image/Certified.png "Certified.png") __This pattern has been certified.__
Related submission, with evaluation history, can be found __here__





#  Graphical representation


__Diagram__




[![Image:timeindexedpartof.jpg](../images/c/c0/Timeindexedpartof.jpg)](../Image/Timeindexedpartof.jpg "Image:timeindexedpartof.jpg")




#  General description


  




#  Elements


_The __TimeIndexedPartOf__ Content OP locally defines the following ontology elements:_




[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif "Class") __Object__ (owl:Class) Any physical, social, or mental object, or a substance 



 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[Object](../Submissions/TimeIndexedPartOf/Object "Submissions:TimeIndexedPartOf/Object") page_

[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif "Class") __Time Indexed Part Of__ (owl:Class) A  [situation](../Submissions/Situation/Situation "Submissions:Situation/Situation") that includes at least two  [Objects](../Submissions/TimeIndexedPartOf/Object "Submissions:TimeIndexedPartOf/Object"), one having the role of whole object, the other(s) being a part(s) of it, and one  [time interval](../Submissions/TimeInterval/TimeInterval "Submissions:TimeInterval/TimeInterval"). 



 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[TimeIndexedPartOf](../Submissions/TimeIndexedPartOf/TimeIndexedPartOf "Submissions:TimeIndexedPartOf/TimeIndexedPartOf") page_

[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif "ObjectProperty") __at time__ (owl:ObjectProperty) A relation between a temporary part-of situation and the time it occurs at. It is a subproperty of  [is setting for](../Submissions/Situation/isSettingFor "Submissions:Situation/isSettingFor"), its domain is the class of  [time indexed part of situations](../Submissions/TimeIndexedPartOf/TimeIndexedPartOf "Submissions:TimeIndexedPartOf/TimeIndexedPartOf"), its range is the class  [time interval](../Submissions/TimeInterval/TimeInterval "Submissions:TimeInterval/TimeInterval"). 



 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[atTime](../Submissions/TimeIndexedPartOf/atTime "Submissions:TimeIndexedPartOf/atTime") page_

[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif "ObjectProperty") __is time of__ (owl:ObjectProperty) The inverse of the  [at time](../Submissions/TimeIndexedPartOf/atTime "Submissions:TimeIndexedPartOf/atTime") object property. 



 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[isTimeOf](../Submissions/TimeIndexedPartOf/isTimeOf "Submissions:TimeIndexedPartOf/isTimeOf") page_

[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif "ObjectProperty") __includes whole object__ (owl:ObjectProperty) A relation between a temporary part-of situation and the whole object involved. It is a subproperty of  [is setting for](../Submissions/Situation/isSettingFor "Submissions:Situation/isSettingFor"), its domain is the class of  [time indexed part of situations](../Submissions/TimeIndexedPartOf/TimeIndexedPartOf "Submissions:TimeIndexedPartOf/TimeIndexedPartOf"), its range is the class  [object](../Submissions/TimeIndexedPartOf/Object "Submissions:TimeIndexedPartOf/Object"). 



 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[includesWholeObject](../Submissions/TimeIndexedPartOf/includesWholeObject "Submissions:TimeIndexedPartOf/includesWholeObject") page_

[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif "ObjectProperty") __is whole object of__ (owl:ObjectProperty) The inverse of the  [includes whole object](../Submissions/TimeIndexedPartOf/includesWholeObject "Submissions:TimeIndexedPartOf/includesWholeObject") property. 



 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[isWholeObjectOf](../Submissions/TimeIndexedPartOf/isWholeObjectOf "Submissions:TimeIndexedPartOf/isWholeObjectOf") page_

[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif "ObjectProperty") __includes part object__ (owl:ObjectProperty) A relation between a temporary part-of situation and the part(s) involved. It is a subproperty of  [is setting for](../Submissions/Situation/isSettingFor "Submissions:Situation/isSettingFor"), its domain is the class of  [time indexed part of situations](../Submissions/TimeIndexedPartOf/TimeIndexedPartOf "Submissions:TimeIndexedPartOf/TimeIndexedPartOf"), its range is the class  [object](../Submissions/TimeIndexedPartOf/Object "Submissions:TimeIndexedPartOf/Object"). 



 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[includesPartObject](../Submissions/TimeIndexedPartOf/includesPartObject "Submissions:TimeIndexedPartOf/includesPartObject") page_

[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif "ObjectProperty") __is part object of__ (owl:ObjectProperty) The inverse of the  [includes part object](../Submissions/TimeIndexedPartOf/includesPartObject "Submissions:TimeIndexedPartOf/includesPartObject") property. 



 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[isPartObjectOf](../Submissions/TimeIndexedPartOf/isPartObjectOf "Submissions:TimeIndexedPartOf/isPartObjectOf") page_
#  Additional information


This Content OP locally defines the above elements, it also includes the elements of  [situation](../Submissions/Situation "Submissions:Situation"), [time interval](../Submissions/TimeInterval "Submissions:TimeInterval"), and  [part of](../Submissions/PartOf "Submissions:PartOf") Content OPs.



#  Scenarios



__Scenarios about TimeIndexedPartOf__
No scenario is added to this Content OP.




#  Reviews



__Reviews about TimeIndexedPartOf__
There is no review about this proposal.
This revision (revision ID __9133__) takes in account the reviews: none


Other info at [evaluation tab](http://ontologydesignpatterns.org/wiki/index.php?title=Submissions:TimeIndexedPartOf&action=evaluation "http://ontologydesignpatterns.org/wiki/index.php?title=Submissions:TimeIndexedPartOf&action=evaluation")




  




#  Modeling issues



__Modeling issues about TimeIndexedPartOf__
There is no Modeling issue related to this proposal.




  




#  References


[Add a reference](index.php@title=Odp%253AAdd_reference&subject=../Submissions/TimeIndexedPartOf "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_reference&subject=Submissions%3ATimeIndexedPartOf")


  






Retrieved from "[http://ontologydesignpatterns.org/wiki/Submissions:TimeIndexedPartOf](../Submissions/TimeIndexedPartOf)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [ProposedContentOP](../Category/ProposedContentOP "Category:ProposedContentOP")