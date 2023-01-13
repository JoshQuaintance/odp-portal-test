[![](../images/thumb/b/b5/Certified.png/70px-Certified.png)](../Image/Certified.png "Certified.png") __This pattern has been certified.__
Related submission, with evaluation history, can be found __here__





#  Graphical representation


__Diagram__




[![Image:Standard-enforcer-pattern.png](../images/d/df/Standard-enforcer-pattern.png)](../Image/Standard-enforcer-pattern.png "Image:Standard-enforcer-pattern.png")




#  General description


  




#  Elements


_The __Standard Enforcer Pattern__ Content OP locally defines the following ontology elements:_



[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif "ObjectProperty") __enforcesGuideline__ (owl:ObjectProperty) 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[enforcesGuideline](../Submissions/Standard_Enforcer_Pattern/enforcesGuideline "Submissions:Standard Enforcer Pattern/enforcesGuideline") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif "ObjectProperty") __enforcesStandard__ (owl:ObjectProperty) 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[enforcesStandard](../Submissions/Standard_Enforcer_Pattern/enforcesStandard "Submissions:Standard Enforcer Pattern/enforcesStandard") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif "ObjectProperty") __guidelinePrescribedIn__ (owl:ObjectProperty) 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[guidelinePrescribedIn](../Submissions/Standard_Enforcer_Pattern/guidelinePrescribedIn "Submissions:Standard Enforcer Pattern/guidelinePrescribedIn") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif "ObjectProperty") __hasDomainScope__ (owl:ObjectProperty) 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[hasDomainScope](../Submissions/Standard_Enforcer_Pattern/hasDomainScope "Submissions:Standard Enforcer Pattern/hasDomainScope") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif "ObjectProperty") __hasProcessScope__ (owl:ObjectProperty) 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[hasProcessScope](../Submissions/Standard_Enforcer_Pattern/hasProcessScope "Submissions:Standard Enforcer Pattern/hasProcessScope") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif "ObjectProperty") __isEnforcedBy__ (owl:ObjectProperty) 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[isEnforcedBy](../Submissions/Standard_Enforcer_Pattern/isEnforcedBy "Submissions:Standard Enforcer Pattern/isEnforcedBy") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif "ObjectProperty") __prescribesGuideline__ (owl:ObjectProperty) 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[prescribesGuideline](../Submissions/Standard_Enforcer_Pattern/prescribesGuideline "Submissions:Standard Enforcer Pattern/prescribesGuideline") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif "Class") __DomainScope__ (owl:Class) An entity that identifies the domain level scope of the standard 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[DomainScope](../Submissions/Standard_Enforcer_Pattern/DomainScope "Submissions:Standard Enforcer Pattern/DomainScope") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif "Class") __Guideline__ (owl:Class) An entity that defines the guideline that is part of a standard 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[Guideline](../Submissions/Standard_Enforcer_Pattern/Guideline "Submissions:Standard Enforcer Pattern/Guideline") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif "Class") __Process__ (owl:Class) An entity that defines a workflow, operation, activity or a service 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[Process](../Submissions/Standard_Enforcer_Pattern/Process "Submissions:Standard Enforcer Pattern/Process") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif "Class") __ProcessEnforcingStandard__ (owl:Class) A process/operation/activity or serrvice that enforces one or more standard. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[ProcessEnforcingStandard](../Submissions/Standard_Enforcer_Pattern/ProcessEnforcingStandard "Submissions:Standard Enforcer Pattern/ProcessEnforcingStandard") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif "Class") __ProcessScope__ (owl:Class) An entity that defines the scope of a process 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[ProcessScope](../Submissions/Standard_Enforcer_Pattern/ProcessScope "Submissions:Standard Enforcer Pattern/ProcessScope") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif "Class") __Standard__ (owl:Class) An entity that identifies a specification established through domain expert consensus that prescribes a set of rules and guidelines for a given context within the domain. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[Standard](../Submissions/Standard_Enforcer_Pattern/Standard "Submissions:Standard Enforcer Pattern/Standard") page_
#  Additional information


This ontology models the standards enforcer pattern (SEP). The main advantage of this pattern is that it provides the capability
to link processes operation and activities to their governing
standards in a generic way. The pattern can be applied to all those
use cases where a standard is enforced.



#  Scenarios



__Scenarios about Standard Enforcer Pattern__
No scenario is added to this Content OP.




#  Reviews



__Reviews about Standard Enforcer Pattern__
This revision (revision ID __11210__) takes in account the reviews: none


Other info at [evaluation tab](http://ontologydesignpatterns.org/wiki/index.php?title=Submissions:Standard_Enforcer_Pattern&action=evaluation "http://ontologydesignpatterns.org/wiki/index.php?title=Submissions:Standard_Enforcer_Pattern&action=evaluation")




  




#  Modeling issues



__Modeling issues about Standard Enforcer Pattern__
There is no Modeling issue related to this proposal.




  




#  References


[Add a reference](index.php@title=Odp%253AAdd_reference&subject=Submissions%253AStandard+Enforcer+Pattern.html "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_reference&subject=Submissions%3AStandard+Enforcer+Pattern")


  






Retrieved from "[http://ontologydesignpatterns.org/wiki/Submissions:Standard\_Enforcer\_Pattern](../Submissions/Standard_Enforcer_Pattern)"
 [Categories](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [ProposedContentOP](../Category/ProposedContentOP "Category:ProposedContentOP") | [Submitted to event](../Category/Submitted_to_event "Category:Submitted to event") | [Review assigned](../Category/Review_assigned "Category:Review assigned")