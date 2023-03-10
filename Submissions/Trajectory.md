[![](../images/thumb/b/b5/Certified.png/70px-Certified.png)](../Image/Certified.png "Certified.png") __This pattern has been certified.__
Related submission, with evaluation history, can be found __here__





#  Graphical representation


__Diagram__




[![Image:Trajectory.png](../images/8/87/Trajectory.png)](../Image/Trajectory.png "Image:Trajectory.png")




#  General description


  




#  Elements


_The __Trajectory__ Content OP locally defines the following ontology elements:_



[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif "ObjectProperty") __atPlace__ (owl:ObjectProperty) Connects anything (including fixes in this pattern) to Place. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[atPlace](../Submissions/Trajectory/atPlace "Submissions:Trajectory/atPlace") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif "ObjectProperty") __atTime__ (owl:ObjectProperty) Connects anything (including fixes in this pattern) to TimeEntity 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[atTime](../Submissions/Trajectory/atTime "Submissions:Trajectory/atTime") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif "ObjectProperty") __endsAt__ (owl:ObjectProperty) Connects a segment to the fix it ends at. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[endsAt](../Submissions/Trajectory/endsAt "Submissions:Trajectory/endsAt") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif "ObjectProperty") __hasAttribute__ (owl:ObjectProperty) Connects a fix or a segment to an additional information as represented by an instance of Attribute. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[hasAttribute](../Submissions/Trajectory/hasAttribute "Submissions:Trajectory/hasAttribute") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif "ObjectProperty") __hasFix__ (owl:ObjectProperty) Relating the trajectory to each of its fixes. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[hasFix](../Submissions/Trajectory/hasFix "Submissions:Trajectory/hasFix") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif "ObjectProperty") __hasSegment__ (owl:ObjectProperty) Relating the trajectory to each of its segments. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[hasSegment](../Submissions/Trajectory/hasSegment "Submissions:Trajectory/hasSegment") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif "ObjectProperty") __hasTrajectory__ (owl:ObjectProperty) Anything that has a trajectory can use this property to connect it to the trajectory instance. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[hasTrajectory](../Submissions/Trajectory/hasTrajectory "Submissions:Trajectory/hasTrajectory") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif "ObjectProperty") __nextFix__ (owl:ObjectProperty) Relates one fix to the immediately following fix in the sequence. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[nextFix](../Submissions/Trajectory/nextFix "Submissions:Trajectory/nextFix") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif "ObjectProperty") __startsFrom__ (owl:ObjectProperty) Connects a segment to the fix it starts from. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[startsFrom](../Submissions/Trajectory/startsFrom "Submissions:Trajectory/startsFrom") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif "ObjectProperty") __traversedBy__ (owl:ObjectProperty) Connect a segment to the moving object that traverses it. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[traversedBy](../Submissions/Trajectory/traversedBy "Submissions:Trajectory/traversedBy") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif "Class") __Attribute__ (owl:Class) Captures additional information that enriches some fix or segment. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[Attribute](../Submissions/Trajectory/Attribute "Submissions:Trajectory/Attribute") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif "Class") __EndingFix__ (owl:Class) The last fix in a particular sequence of fixes. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[EndingFix](../Submissions/Trajectory/EndingFix "Submissions:Trajectory/EndingFix") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif "Class") __Fix__ (owl:Class) Describes a fix, which is an adorned spatiotemporal point. A sequence of fixes form the trajectory. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[Fix](../Submissions/Trajectory/Fix "Submissions:Trajectory/Fix") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif "Class") __MovingObject__ (owl:Class) This is the hook to an ontology/pattern that describes the moving object, if any, which moves along the trajectory. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[MovingObject](../Submissions/Trajectory/MovingObject "Submissions:Trajectory/MovingObject") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif "Class") __Place__ (owl:Class) This is the hook to other pattern/ontology that describes the notion of place, which is more general than just a location/geo-coordinate. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[Place](../Submissions/Trajectory/Place "Submissions:Trajectory/Place") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif "Class") __Segment__ (owl:Class) The Segment class captures the "connection" between two consecutive fixes. That is, a segment starts from a fix and ends at another fix. If the pattern is used to model the trajectory of some moving object, each segment is traversed by that moving object. Additional information about a segment can be attached as attributes. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[Segment](../Submissions/Trajectory/Segment "Submissions:Trajectory/Segment") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif "Class") __StartingFix__ (owl:Class) The first fix in a particular sequence of fixes. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[StartingFix](../Submissions/Trajectory/StartingFix "Submissions:Trajectory/StartingFix") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif "Class") __TimeEntity__ (owl:Class) The hook to class/pattern/ontology that models time, this class provides the temporal extent of the trajectory. One example of time model is the W3C Time Ontology. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[TimeEntity](../Submissions/Trajectory/TimeEntity "Submissions:Trajectory/TimeEntity") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif "Class") __Trajectory__ (owl:Class) Represents the notion of trajectory, this is the main class that can be hooked with other patterns that use the Trajectory pattern. Trajectory in this model is understood as a sequence of fixes connected by segments. There is exactly one starting fix and exactly one ending fix. Each fix has a temporal extent and a place (which is more general than just a location). 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[Trajectory](../Submissions/Trajectory/Trajectory "Submissions:Trajectory/Trajectory") page_
#  Additional information


#  Scenarios



__Scenarios about Trajectory__
No scenario is added to this Content OP.




#  Reviews



__Reviews about Trajectory__
There is no review about this proposal.
This revision (revision ID __12794__) takes in account the reviews: none


Other info at [evaluation tab](http://ontologydesignpatterns.org/wiki/index.php?title=Submissions:Trajectory&action=evaluation "http://ontologydesignpatterns.org/wiki/index.php?title=Submissions:Trajectory&action=evaluation")




  




#  Modeling issues



__Modeling issues about Trajectory__
There is no Modeling issue related to this proposal.




  




#  References


[Add a reference](index.php@title=Odp%253AAdd_reference&subject=../Submissions/Trajectory "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_reference&subject=Submissions%3ATrajectory")


  






Retrieved from "[http://ontologydesignpatterns.org/wiki/Submissions:Trajectory](../Submissions/Trajectory)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [ProposedContentOP](../Category/ProposedContentOP "Category:ProposedContentOP")