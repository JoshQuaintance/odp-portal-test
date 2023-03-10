[![](../images/thumb/b/b5/Certified.png/70px-Certified.png)](../Image/Certified.png "Certified.png") __This pattern has been certified.__
Related submission, with evaluation history, can be found __here__





#  Graphical representation


__Diagram__




[![Image:Reactor-pattern.png](../images/4/4b/Reactor-pattern.png)](../Image/Reactor-pattern.png "Image:Reactor-pattern.png")




#  General description


  




#  Elements


_The __Reactor pattern__ Content OP locally defines the following ontology elements:_



 [![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif "ObjectProperty") __definesCondition__ (owl:ObjectProperty) 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[definesCondition](../Submissions/Reactor_pattern/definesCondition "Submissions:Reactor pattern/definesCondition") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif "ObjectProperty") __hasEnvironemntalCondition__ (owl:ObjectProperty) 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[hasEnvironemntalCondition](../Submissions/Reactor_pattern/hasEnvironemntalCondition "Submissions:Reactor pattern/hasEnvironemntalCondition") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif "ObjectProperty") __hasInputParameter__ (owl:ObjectProperty) 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[hasInputParameter](../Submissions/Reactor_pattern/hasInputParameter "Submissions:Reactor pattern/hasInputParameter") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif "ObjectProperty") __hasMeasurement__ (owl:ObjectProperty) 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[hasMeasurement](../Submissions/Reactor_pattern/hasMeasurement "Submissions:Reactor pattern/hasMeasurement") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif "ObjectProperty") __hasOutputParameter__ (owl:ObjectProperty) 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[hasOutputParameter](../Submissions/Reactor_pattern/hasOutputParameter "Submissions:Reactor pattern/hasOutputParameter") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif "ObjectProperty") __hasProcessParameter__ (owl:ObjectProperty) 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[hasProcessParameter](../Submissions/Reactor_pattern/hasProcessParameter "Submissions:Reactor pattern/hasProcessParameter") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif "ObjectProperty") __triggeredBy__ (owl:ObjectProperty) 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[triggeredBy](../Submissions/Reactor_pattern/triggeredBy "Submissions:Reactor pattern/triggeredBy") page_
[![DatatypeProperty](../images/thumb/a/a5/DatatypeProperty.gif/20px-DatatypeProperty.gif)](../Image/DatatypeProperty.gif "DatatypeProperty") __hasDescription__ (owl:DatatypeProperty) 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[hasDescription](../Submissions/Reactor_pattern/hasDescription "Submissions:Reactor pattern/hasDescription") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif "Class") __EnvironmentalCondition__ (owl:Class) An entity that represents the environmental condition 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[EnvironmentalCondition](../Submissions/Reactor_pattern/EnvironmentalCondition "Submissions:Reactor pattern/EnvironmentalCondition") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif "Class") __Event__ (owl:Class) An entity representing the event that triggers the process 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[Event](../Submissions/Reactor_pattern/Event "Submissions:Reactor pattern/Event") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif "Class") __InputParameter__ (owl:Class) An entity representing the input to a process 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[InputParameter](../Submissions/Reactor_pattern/InputParameter "Submissions:Reactor pattern/InputParameter") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif "Class") __OutputParameter__ (owl:Class) An entity representing the output to a process 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[OutputParameter](../Submissions/Reactor_pattern/OutputParameter "Submissions:Reactor pattern/OutputParameter") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif "Class") __Process__ (owl:Class) An entity representing a placeholder for a process. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[Process](../Submissions/Reactor_pattern/Process "Submissions:Reactor pattern/Process") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif "Class") __ProcessParameter__ (owl:Class) An overarching entity representing the parameters defined for the process 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[ProcessParameter](../Submissions/Reactor_pattern/ProcessParameter "Submissions:Reactor pattern/ProcessParameter") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif "Class") __ReactiveProcess__ (owl:Class) An entity representing a reactive process 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[ReactiveProcess](../Submissions/Reactor_pattern/ReactiveProcess "Submissions:Reactor pattern/ReactiveProcess") page_
#  Additional information


The Reactor Pattern enables the modelling of processes that consume inputs and produce outputs under specific environmental conditions and on being triggered by certain events. Reactor pattern is a content ontology design pattern and is especially targeted towards modelling reactive processes with a black box view of the process.



#  Scenarios



__Scenarios about Reactor pattern__
No scenario is added to this Content OP.




#  Reviews



__Reviews about Reactor pattern__
This revision (revision ID __11175__) takes in account the reviews: none


Other info at [evaluation tab](http://ontologydesignpatterns.org/wiki/index.php?title=Submissions:Reactor_pattern&action=evaluation "http://ontologydesignpatterns.org/wiki/index.php?title=Submissions:Reactor_pattern&action=evaluation")




  




#  Modeling issues



__Modeling issues about Reactor pattern__
There is no Modeling issue related to this proposal.




  




#  References


[Add a reference](index.php@title=Odp%253AAdd_reference&subject=Submissions%253AReactor+pattern.html "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_reference&subject=Submissions%3AReactor+pattern")


  






Retrieved from "[http://ontologydesignpatterns.org/wiki/Submissions:Reactor\_pattern](../Submissions/Reactor_pattern)"
 [Categories](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [ProposedContentOP](../Category/ProposedContentOP "Category:ProposedContentOP") | [Submitted to event](../Category/Submitted_to_event "Category:Submitted to event") | [Review assigned](../Category/Review_assigned "Category:Review assigned")