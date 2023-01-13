[![](../images/thumb/b/b5/Certified.png/70px-Certified.png)](../Image/Certified.png.md "Certified.png") __This pattern has been certified.__
Related submission, with evaluation history, can be found __here__





#  Graphical representation


__Diagram__




[![Image:ODP_new.png](../images/f/f8/ODP_new.png)](../Image/ODP_new.png.md "Image:ODP_new.png")




#  General description


  




#  Elements


_The __Pollution__ Content OP locally defines the following ontology elements:_



__Authors__ (owl:AnnotationProperty) 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[Authors](../Submissions/Pollution/Authors.md "Submissions:Pollution/Authors") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __atPlace__ (owl:ObjectProperty) 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[atPlace](../Submissions/Pollution/atPlace.md "Submissions:Pollution/atPlace") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __atTime__ (owl:ObjectProperty) 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[atTime](../Submissions/Pollution/atTime.md "Submissions:Pollution/atTime") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __carriesPollutant__ (owl:ObjectProperty) 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[carriesPollutant](../Submissions/Pollution/carriesPollutant.md "Submissions:Pollution/carriesPollutant") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __endsAt__ (owl:ObjectProperty) Connects a segment to the point it ends at. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[endsAt](../Submissions/Pollution/endsAt.md "Submissions:Pollution/endsAt") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __hasContributor__ (owl:ObjectProperty) 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[hasContributor](../Submissions/Pollution/hasContributor.md "Submissions:Pollution/hasContributor") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __hasObservation__ (owl:ObjectProperty) 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[hasObservation](../Submissions/Pollution/hasObservation.md "Submissions:Pollution/hasObservation") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __hasPoint__ (owl:ObjectProperty) Relating the trajectory to each of its points. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[hasPoint](../Submissions/Pollution/hasPoint.md "Submissions:Pollution/hasPoint") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __hasPrescribedStandard__ (owl:ObjectProperty) 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[hasPrescribedStandard](../Submissions/Pollution/hasPrescribedStandard.md "Submissions:Pollution/hasPrescribedStandard") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __hasSegment__ (owl:ObjectProperty) Relating the trajectory to each of its segments. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[hasSegment](../Submissions/Pollution/hasSegment.md "Submissions:Pollution/hasSegment") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __hasTrajectory__ (owl:ObjectProperty) Anything that has a trajectory can use this property to connect it to the trajectory instance 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[hasTrajectory](../Submissions/Pollution/hasTrajectory.md "Submissions:Pollution/hasTrajectory") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __nextPoint__ (owl:ObjectProperty) Relates one point to the immediately following point in the sequence. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[nextPoint](../Submissions/Pollution/nextPoint.md "Submissions:Pollution/nextPoint") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __startsFrom__ (owl:ObjectProperty) Connects a segment to the point it starts from. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[startsFrom](../Submissions/Pollution/startsFrom.md "Submissions:Pollution/startsFrom") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif.md "Class") __Carrier__ (owl:Class) Represents streams which carry pollutants to a particular place. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[Carrier](../Submissions/Pollution/Carrier.md "Submissions:Pollution/Carrier") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif.md "Class") __Contributor__ (owl:Class) 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[Contributor](../Submissions/Pollution/Contributor.md "Submissions:Pollution/Contributor") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif.md "Class") __DirectContributor__ (owl:Class) Represents concepts which directly represent pollution. For example the concentration of pollutants at a particular spatio-temporal point. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[DirectContributor](../Submissions/Pollution/DirectContributor.md "Submissions:Pollution/DirectContributor") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif.md "Class") __EndingPoint__ (owl:Class) 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[EndingPoint](../Submissions/Pollution/EndingPoint.md "Submissions:Pollution/EndingPoint") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif.md "Class") __IndirectContributor__ (owl:Class) Represents concepts which indirectly contribute to pollution of a place. These do not directly represent pollution but have properties which can affect the pollution, for example by changing the concentration of pollutants at a spatio-temporal point. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[IndirectContributor](../Submissions/Pollution/IndirectContributor.md "Submissions:Pollution/IndirectContributor") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif.md "Class") __NaturalResourcePollution__ (owl:Class) Represents pollution on natural resources. Which means the pollution that affects natural resources like air, water, land, etc. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[NaturalResourcePollution](../Submissions/Pollution/NaturalResourcePollution.md "Submissions:Pollution/NaturalResourcePollution") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif.md "Class") __NonNaturalResourcePollution__ (owl:Class) Represents pollution which does not represent natural resource. Examples include, sound, light, space debris, radioactive pollution, thermal pollution. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[NonNaturalResourcePollution](../Submissions/Pollution/NonNaturalResourcePollution.md "Submissions:Pollution/NonNaturalResourcePollution") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif.md "Class") __Observation__ (owl:Class) Observation represents a spatio-temporal observation of pollutants under time and place parameters. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[Observation](../Submissions/Pollution/Observation.md "Submissions:Pollution/Observation") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif.md "Class") __PlaceEntity__ (owl:Class) 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[PlaceEntity](../Submissions/Pollution/PlaceEntity.md "Submissions:Pollution/PlaceEntity") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif.md "Class") __Pollutant__ (owl:Class) Represents various pollutants which contaminate the environment and directly represnt/contribute to pollution. Additionally a carrier's trajecectory point may pick up pollutants from a spatio-temporal point, in which case, it is represented by the sub-property carriesPollutant. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[Pollutant](../Submissions/Pollution/Pollutant.md "Submissions:Pollution/Pollutant") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif.md "Class") __Pollution__ (owl:Class) Represnents the notion of Pollution which includes observation of pollutants at spatio-temporal points or the contributors to the pollution which may be spatio-temporal in nature. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[Pollution](../Submissions/Pollution/Pollution.md "Submissions:Pollution/Pollution") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif.md "Class") __PrescribedStandardForPollutant__ (owl:Class) 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[PrescribedStandardForPollutant](../Submissions/Pollution/PrescribedStandardForPollutant.md "Submissions:Pollution/PrescribedStandardForPollutant") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif.md "Class") __StartingPoint__ (owl:Class) 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[StartingPoint](../Submissions/Pollution/StartingPoint.md "Submissions:Pollution/StartingPoint") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif.md "Class") __TimeEntity__ (owl:Class) 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[TimeEntity](../Submissions/Pollution/TimeEntity.md "Submissions:Pollution/TimeEntity") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif.md "Class") __Trajectory__ (owl:Class) Represents a trajectory of points. Examples include drainage/sewage trajectory or air stream trajectory. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[Trajectory](../Submissions/Pollution/Trajectory.md "Submissions:Pollution/Trajectory") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif.md "Class") __TrajectoryPoint__ (owl:Class) A collection of spatio-temporal points represents a trajectory 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[TrajectoryPoint](../Submissions/Pollution/TrajectoryPoint.md "Submissions:Pollution/TrajectoryPoint") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif.md "Class") __TrajectorySegment__ (owl:Class) A subset of spatio-temporal trajectory points represent a TrajectorySegment 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[TrajectorySegment](../Submissions/Pollution/TrajectorySegment.md "Submissions:Pollution/TrajectorySegment") page_
#  Additional information


This ontology is an attempt at a ODP designed to model Pollution. Pollution can be defined as



#  Scenarios



__Scenarios about Pollution__
No scenario is added to this Content OP.




#  Reviews



__Reviews about Pollution__
There is no review about this proposal.
This revision (revision ID __14244__) takes in account the reviews: none


Other info at [evaluation tab](http://ontologydesignpatterns.org/wiki/index.php?title=Submissions:Pollution&action=evaluation "http://ontologydesignpatterns.org/wiki/index.php?title=Submissions:Pollution&action=evaluation")




  




#  Modeling issues



__Modeling issues about Pollution__
There is no Modeling issue related to this proposal.




  




#  References


[Add a reference](index.php@title=Odp%253AAdd_reference&subject=../Submissions/Pollution.md "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_reference&subject=Submissions%3APollution")


  






Retrieved from "[http://ontologydesignpatterns.org/wiki/Submissions:Pollution](../Submissions/Pollution.md)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [ProposedContentOP](../Category/ProposedContentOP.md "Category:ProposedContentOP")