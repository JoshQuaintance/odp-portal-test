[![](../images/thumb/b/b5/Certified.png/70px-Certified.png)](../Image/Certified.png "Certified.png") __This pattern has been certified.__
Related submission, with evaluation history, can be found __here__





#  Graphical representation


__Diagram__




[![Image:LCAFlow.png](../images/4/4b/LCAFlow.png)](../Image/LCAFlow.png "Image:LCAFlow.png")




#  General description


  




#  Elements


_The __LCA Pattern__ Content OP locally defines the following ontology elements:_



[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif "ObjectProperty") __hasCompartment__ (owl:ObjectProperty) 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[hasCompartment](../Submissions/LCA_Pattern/hasCompartment "Submissions:LCA Pattern/hasCompartment") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif "ObjectProperty") __hasLocation__ (owl:ObjectProperty) 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[hasLocation](../Submissions/LCA_Pattern/hasLocation "Submissions:LCA Pattern/hasLocation") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif "ObjectProperty") __hasProperty__ (owl:ObjectProperty) 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[hasProperty](../Submissions/LCA_Pattern/hasProperty "Submissions:LCA Pattern/hasProperty") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif "ObjectProperty") __hasTemporalExtent__ (owl:ObjectProperty) 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[hasTemporalExtent](../Submissions/LCA_Pattern/hasTemporalExtent "Submissions:LCA Pattern/hasTemporalExtent") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif "ObjectProperty") __isInputOf__ (owl:ObjectProperty) 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[isInputOf](../Submissions/LCA_Pattern/isInputOf "Submissions:LCA Pattern/isInputOf") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif "ObjectProperty") __isOutputOf__ (owl:ObjectProperty) 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[isOutputOf](../Submissions/LCA_Pattern/isOutputOf "Submissions:LCA Pattern/isOutputOf") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif "ObjectProperty") __performs__ (owl:ObjectProperty) 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[performs](../Submissions/LCA_Pattern/performs "Submissions:LCA Pattern/performs") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif "ObjectProperty") __playsRoleOf__ (owl:ObjectProperty) 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[playsRoleOf](../Submissions/LCA_Pattern/playsRoleOf "Submissions:LCA Pattern/playsRoleOf") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif "Class") __Activity__ (owl:Class) Each activity is performed by at least one agent such as an coal power plant that performs the generation of electricity. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[Activity](../Submissions/LCA_Pattern/Activity "Submissions:LCA Pattern/Activity") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif "Class") __Agent__ (owl:Class) 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[Agent](../Submissions/LCA_Pattern/Agent "Submissions:LCA Pattern/Agent") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif "Class") __Compartment__ (owl:Class) 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[Compartment](../Submissions/LCA_Pattern/Compartment "Submissions:LCA Pattern/Compartment") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif "Class") __ElementaryFlow__ (owl:Class) It describes material or energy that is entering the system from the environment without any previous transformation by humans or is leaving the system by being released into the environment without further human transformation 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[ElementaryFlow](../Submissions/LCA_Pattern/ElementaryFlow "Submissions:LCA Pattern/ElementaryFlow") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif "Class") __Flow__ (owl:Class) Flows are streams of material or energy that can act as the inputs and outputs of activities. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[Flow](../Submissions/LCA_Pattern/Flow "Submissions:LCA Pattern/Flow") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif "Class") __IntermediateFlow__ (owl:Class) Intermediate flows occur between processes of the studied system. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[IntermediateFlow](../Submissions/LCA_Pattern/IntermediateFlow "Submissions:LCA Pattern/IntermediateFlow") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif "Class") __Location__ (owl:Class) 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[Location](../Submissions/LCA_Pattern/Location "Submissions:LCA Pattern/Location") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif "Class") __Product__ (owl:Class) 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[Product](../Submissions/LCA_Pattern/Product "Submissions:LCA Pattern/Product") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif "Class") __Property__ (owl:Class) 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[Property](../Submissions/LCA_Pattern/Property "Submissions:LCA Pattern/Property") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif "Class") __ReferencedProduct__ (owl:Class) 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[ReferencedProduct](../Submissions/LCA_Pattern/ReferencedProduct "Submissions:LCA Pattern/ReferencedProduct") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif "Class") __Time__ (owl:Class) 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[Time](../Submissions/LCA_Pattern/Time "Submissions:LCA Pattern/Time") page_
__air__ (owl:NamedIndividual) 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[air](../Submissions/LCA_Pattern/air "Submissions:LCA Pattern/air") page_
__soil__ (owl:NamedIndividual) 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[soil](../Submissions/LCA_Pattern/soil "Submissions:LCA Pattern/soil") page_
__water__ (owl:NamedIndividual) 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[water](../Submissions/LCA_Pattern/water "Submissions:LCA Pattern/water") page_
#  Additional information


In a nutshell, estimating the environmental impact of a certain product requires an understanding of all impacts accumulated during the creation, lifetime, and decommissioning of said product. With respect to the solar panel example introduced in our related paper, the creation of the solar arrays requires multiple activities such as the transportation of resources, the generation of electric power by a coal power plant necessary to manufacture certain parts of the panels, or the disposal of polluted sludge accumulated during the production. In other words, the Eco-efficiency of solar panels depends on the activities involved in all stages of their life-cycle.



#  Scenarios



__Scenarios about LCA Pattern__
No scenario is added to this Content OP.




#  Reviews



__Reviews about LCA Pattern__
There is no review about this proposal.
This revision (revision ID __12311__) takes in account the reviews: none


Other info at [evaluation tab](http://ontologydesignpatterns.org/wiki/index.php?title=Submissions:LCA_Pattern&action=evaluation "http://ontologydesignpatterns.org/wiki/index.php?title=Submissions:LCA_Pattern&action=evaluation")




  




#  Modeling issues



__Modeling issues about LCA Pattern__
There is no Modeling issue related to this proposal.




  




#  References


[Add a reference](index.php@title=Odp%253AAdd_reference&subject=Submissions%253ALCA+Pattern.html "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_reference&subject=Submissions%3ALCA+Pattern")


  






Retrieved from "[http://ontologydesignpatterns.org/wiki/Submissions:LCA\_Pattern](../Submissions/LCA_Pattern)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [ProposedContentOP](../Category/ProposedContentOP "Category:ProposedContentOP")