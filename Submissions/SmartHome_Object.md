[![](../images/thumb/b/b5/Certified.png/70px-Certified.png)](../Image/Certified.png "Certified.png") __This pattern has been certified.__
Related submission, with evaluation history, can be found __here__





#  Graphical representation


__Diagram__
_(this article has no graphical representation)_



#  General description


  




#  Elements


_The __SmartHome Object__ Content OP locally defines the following ontology elements:_



[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif "Class") __Location__ (owl:Class) 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[Location](../Submissions/SmartHome_Object/Location "Submissions:SmartHome Object/Location") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif "Class") __MobileObject__ (owl:Class) 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[MobileObject](../Submissions/SmartHome_Object/MobileObject "Submissions:SmartHome Object/MobileObject") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif "Class") __NodeHolder__ (owl:Class) 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[NodeHolder](../Submissions/SmartHome_Object/NodeHolder "Submissions:SmartHome Object/NodeHolder") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif "Class") __NonMobileObject__ (owl:Class) 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[NonMobileObject](../Submissions/SmartHome_Object/NonMobileObject "Submissions:SmartHome Object/NonMobileObject") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif "Class") __SmartHomeAgent__ (owl:Class) 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[SmartHomeAgent](../Submissions/SmartHome_Object/SmartHomeAgent "Submissions:SmartHome Object/SmartHomeAgent") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif "Class") __SmartHomeObject__ (owl:Class) 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[SmartHomeObject](../Submissions/SmartHome_Object/SmartHomeObject "Submissions:SmartHome Object/SmartHomeObject") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif "Class") __SmartObject__ (owl:Class) 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[SmartObject](../Submissions/SmartHome_Object/SmartObject "Submissions:SmartHome Object/SmartObject") page_
#  Additional information


#  Scenarios



__Scenarios about SmartHome Object__
No scenario is added to this Content OP.




#  Reviews



__Reviews about SmartHome Object__
There is no review about this proposal.
This revision (revision ID __13011__) takes in account the reviews: none


Other info at [evaluation tab](http://ontologydesignpatterns.org/wiki/index.php?title=Submissions:SmartHome_Object&action=evaluation "http://ontologydesignpatterns.org/wiki/index.php?title=Submissions:SmartHome_Object&action=evaluation")




#  Modeling issues



__Modeling issues about SmartHome Object__
There is no Modeling issue related to this proposal.




#  References


[Add a reference](index.php@title=Odp%253AAdd_reference&subject=Submissions%253ASmartHome+Object.html "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_reference&subject=Submissions%3ASmartHome+Object")


  

This pattern relies on both the SSN ontology and DUL in order to represent an object in the context of Smart Home. Using this model we categorize the objects in to two groups of Smart Objects and NodeHolder based on the reason behind their existance in a smart home. 


Due to usual difficulties to install sensors in a smart home environment it is common that some other objects (i.e. NodeHolder) are used to attache sensors on so as to observe the situation of other objects (i.e. SmartObject) specifically for the configuration planner. Using this pattern we are able to diffrentiate between these two types of objects.


This pattern also allows us to extend the definition of an object's properties in the context of smart home. The properties of a SmartObject which are the interest of the sensing process can be defined as either a subclass of the class [http://purl.oclc.org/NET/ssnx/ssn#Property](http://purl.oclc.org/NET/ssnx/ssn#Property "http://purl.oclc.org/NET/ssnx/ssn#Property") (e.g. the temperature of a stove) or as part of the smart object (e.g. the door of a friedge)





Retrieved from "[http://ontologydesignpatterns.org/wiki/Submissions:SmartHome\_Object](../Submissions/SmartHome_Object)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [ProposedContentOP](../Category/ProposedContentOP "Category:ProposedContentOP")