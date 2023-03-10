[![](../images/thumb/b/b5/Certified.png/70px-Certified.png)](../Image/Certified.png "Certified.png") __This pattern has been certified.__
Related submission, with evaluation history, can be found __here__





#  Graphical representation


__Diagram__
_(this article has no graphical representation)_



#  General description


  




#  Elements


_The __BasicPlan__ Content OP locally defines the following ontology elements:_



[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif "ObjectProperty") __conceptualizes__ (owl:ObjectProperty) A relation stating that an Agent is internally representing a SocialObject . E.g., 'John believes in the conspiracy theory'; 'Niels Bohr created the solar-system metaphor for the atomic theory'; 'Jacques assumes all swans are white'; 'the task force members share the attack plan'. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[conceptualizes](../Submissions/BasicPlan/conceptualizes "Submissions:BasicPlan/conceptualizes") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif "ObjectProperty") __executesTask__ (owl:ObjectProperty) A relation between an action and a task, e.g. 'putting some water in a pot and putting the pot on a fire until the water starts bubbling' executes the task 'boiling'. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[executesTask](../Submissions/BasicPlan/executesTask "Submissions:BasicPlan/executesTask") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif "ObjectProperty") __isConceptualizedBy__ (owl:ObjectProperty) A relation stating that an Agent is internally representing a Description . E.g., 'John believes in the conspiracy theory'; 'Niels Bohr created a solar-system metaphor for his atomic theory'; 'Jacques assumes all swans are white'; 'the task force shares the attack plan'. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[isConceptualizedBy](../Submissions/BasicPlan/isConceptualizedBy "Submissions:BasicPlan/isConceptualizedBy") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif "ObjectProperty") __isExecutedIn__ (owl:ObjectProperty) A relation between an action and a task, e.g. 'putting some water in a pot and putting the pot on a fire until the water starts bubbling' executes the task 'boiling'. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[isExecutedIn](../Submissions/BasicPlan/isExecutedIn "Submissions:BasicPlan/isExecutedIn") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif "ObjectProperty") __isParametrizedBy__ (owl:ObjectProperty) The relation between a Parameter, e.g. 'MajorAge', and a Region, e.g. '>17 year'. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[isParametrizedBy](../Submissions/BasicPlan/isParametrizedBy "Submissions:BasicPlan/isParametrizedBy") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif "ObjectProperty") __isSatisfiedBy__ (owl:ObjectProperty) A relation between a Situation and a Description, e.g. the execution of a Plan satisfies that plan. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[isSatisfiedBy](../Submissions/BasicPlan/isSatisfiedBy "Submissions:BasicPlan/isSatisfiedBy") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif "ObjectProperty") __parametrizes__ (owl:ObjectProperty) The relation between a Parameter, e.g. 'MajorAgeLimit', and a Region, e.g. '18\_year'.
For a more data-oriented relation, see hasDataValue 



 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[parametrizes](../Submissions/BasicPlan/parametrizes "Submissions:BasicPlan/parametrizes") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif "ObjectProperty") __satisfies__ (owl:ObjectProperty) A relation between a Situation and a Description, e.g. the execution of a Plan satisfies that plan. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[satisfies](../Submissions/BasicPlan/satisfies "Submissions:BasicPlan/satisfies") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif "Class") __GoalSituation__ (owl:Class) A goal situation is a situation that satisfies a goal.Opposite to the case of subplan executions, a goal situation is not part of a plan execution.In other words, it is not true in general that any situation satisfying a part of a description, is also part of the situation that satisfies the whole description. This helps to account for the following cases: a) Execution of plans containing abort or suspension conditions (the plan would be satisfied even if the goal has not been reached, see below), b) Incidental satisfaction, like when a situation satisfies a goal without being intentionally planned (but anyway desired). 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[GoalSituation](../Submissions/BasicPlan/GoalSituation "Submissions:BasicPlan/GoalSituation") page_
#  Additional information


The basic plans. This content ontology design patterns represents plans descriptions and their executions. It is defined by combining and expanding other CPs: basic plans description, basic plans execution, and object role. Expansion involves the partial clone of ontology elements from DOLCE Ultra Lite and Plans Lite ontologies.



#  Scenarios



__Scenarios about BasicPlan__
No scenario is added to this Content OP.




#  Reviews



__Reviews about BasicPlan__
There is no review about this proposal.
This revision (revision ID __9066__) takes in account the reviews: none


Other info at [evaluation tab](http://ontologydesignpatterns.org/wiki/index.php?title=Submissions:BasicPlan&action=evaluation "http://ontologydesignpatterns.org/wiki/index.php?title=Submissions:BasicPlan&action=evaluation")




  




#  Modeling issues



__Modeling issues about BasicPlan__
There is no Modeling issue related to this proposal.




  




#  References


[Add a reference](index.php@title=Odp%253AAdd_reference&subject=../Submissions/BasicPlan "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_reference&subject=Submissions%3ABasicPlan")


  






Retrieved from "[http://ontologydesignpatterns.org/wiki/Submissions:BasicPlan](../Submissions/BasicPlan)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [ProposedContentOP](../Category/ProposedContentOP "Category:ProposedContentOP")