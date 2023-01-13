[![](../images/thumb/b/b5/Certified.png/70px-Certified.png)](../Image/Certified.png.md "Certified.png") __This pattern has been certified.__
Related submission, with evaluation history, can be found __here__





#  Graphical representation


__Diagram__




[![Image:Transition.png](../images/7/7a/Transition.png)](../Image/Transition.png.md "Image:Transition.png")




#  General description


  




#  Elements


_The __Transition__ Content OP locally defines the following ontology elements:_



[![ObjectProperty](../../../../../../../../../../../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __hasEventAtTime__ (owl:ObjectProperty) The time of the event causing the transition. 
 [![](../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[hasEventAtTime](../Submissions/Transition/hasEventAtTime.md "Submissions:Transition/hasEventAtTime") page_
[![ObjectProperty](../../../../../../../../../../../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __hasFinalStateAtTime__ (owl:ObjectProperty) The time of the final state of the transition. 
 [![](../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[hasFinalStateAtTime](../Submissions/Transition/hasFinalStateAtTime.md "Submissions:Transition/hasFinalStateAtTime") page_
[![ObjectProperty](../../../../../../../../../../../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __hasInitialStateAtTime__ (owl:ObjectProperty) The time of the initial state in the transition. 
 [![](../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[hasInitialStateAtTime](../Submissions/Transition/hasInitialStateAtTime.md "Submissions:Transition/hasInitialStateAtTime") page_
[![ObjectProperty](../../../../../../../../../../../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __includesFinalSituation__ (owl:ObjectProperty) A relation between a transition situation and the situation resulting from the transition. 
 [![](../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[includesFinalSituation](../Submissions/Transition/includesFinalSituation.md "Submissions:Transition/includesFinalSituation") page_
[![ObjectProperty](../../../../../../../../../../../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __includesInitialSituation__ (owl:ObjectProperty) A relation between a transition situation and the situation existing before the transition event. 
 [![](../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[includesInitialSituation](../Submissions/Transition/includesInitialSituation.md "Submissions:Transition/includesInitialSituation") page_
[![ObjectProperty](../../../../../../../../../../../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __includesProcess__ (owl:ObjectProperty) A relation between a transition situation and the underlying process that is invariant for the object(s) included in the transition. 
 [![](../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[includesProcess](../Submissions/Transition/includesProcess.md "Submissions:Transition/includesProcess") page_
[![ObjectProperty](../../../../../../../../../../../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __isFinalSituationIncludedIn__ (owl:ObjectProperty) A relation between a transition situation and the situation resulting from the transition. 
 [![](../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[isFinalSituationIncludedIn](../Submissions/Transition/isFinalSituationIncludedIn.md "Submissions:Transition/isFinalSituationIncludedIn") page_
[![ObjectProperty](../../../../../../../../../../../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __isInitialSituationIncludedIn__ (owl:ObjectProperty) A relation between a transition situation and the situation existing before the transition event. 
 [![](../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[isInitialSituationIncludedIn](../Submissions/Transition/isInitialSituationIncludedIn.md "Submissions:Transition/isInitialSituationIncludedIn") page_
[![ObjectProperty](../../../../../../../../../../../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __isProcessIncludedIn__ (owl:ObjectProperty) A relation between a transition situation and the underlying process that is invariant for the object(s) included in the transition. 
 [![](../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[isProcessIncludedIn](../Submissions/Transition/isProcessIncludedIn.md "Submissions:Transition/isProcessIncludedIn") page_
[![ObjectProperty](../../../../../../../../../../../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __isTimeOf__ (owl:ObjectProperty) 
 [![](../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[isTimeOf](../Submissions/Transition/isTimeOf.md "Submissions:Transition/isTimeOf") page_
[![ObjectProperty](../../../../../../../../../../../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __occursAt__ (owl:ObjectProperty) 
 [![](../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[occursAt](../Submissions/Transition/occursAt.md "Submissions:Transition/occursAt") page_
[![Class](../../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif.md "Class") __Process__ (owl:Class) The invariance under some different transitions (including the one represented here), in which at least one Object is situated. 
 [![](../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[Process](../Submissions/Transition/Process.md "Submissions:Transition/Process") page_
[![Class](../../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif.md "Class") __Transition__ (owl:Class) In this pattern, it is the entity that is invariant across the Process underlying the transition, but is also changed from an initial to a final state by an Event.
  



A transition is a Situation that creates a context for three TimeInterval(s), two additional different Situation(s), one Event, one Process, and at least one Object: the Event is observed as the cause for the transition, one Situation is the state before the transition, the second Situation is the state after the transition, the Process is the invariance under some different transitions (including the one represented here), in which at least one Object is situated. Finally, the time intervals position the situations and the transitional event in time.


This class of situations partly encodes the ontology underlying typical engineering algebras for processes, e.g. Petri Nets. 


A full representation of the transition ontology is outside the expressivity of OWL, because we would need qualified cardinality restrictions, coreference, property equivalence, and property composition. 



 [![](../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[Transition](../Submissions/Transition/Transition.md "Submissions:Transition/Transition") page_
#  Additional information


A simple pattern to represent transitions between states.



#  Scenarios



__Scenarios about Transition__
No scenario is added to this Content OP.




#  Reviews



__Reviews about Transition__
There is no review about this proposal.
This revision (revision ID __9137__) takes in account the reviews: none


Other info at [evaluation tab](http://ontologydesignpatterns.org/wiki/index.php?title=Submissions:Transition&action=evaluation "http://ontologydesignpatterns.org/wiki/index.php?title=Submissions:Transition&action=evaluation")




  




#  Modeling issues



__Modeling issues about Transition__
There is no Modeling issue related to this proposal.




  




#  References


[Add a reference](index.php@title=Odp%253AAdd_reference&subject=../Submissions/Transition.md "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_reference&subject=Submissions%3ATransition")


  






Retrieved from "[http://ontologydesignpatterns.org/wiki/Submissions:Transition](../Submissions/Transition.md)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [ProposedContentOP](../Category/ProposedContentOP.md "Category:ProposedContentOP")