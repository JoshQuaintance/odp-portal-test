[![](../images/thumb/b/b5/Certified.png/70px-Certified.png)](../Image/Certified.png.md "Certified.png") __This pattern has been certified.__
Related submission, with evaluation history, can be found __here__





#  Graphical representation


__Diagram__
_(this article has no graphical representation)_



#  General description


  




#  Elements


_The __ActingFor__ Content OP locally defines the following ontology elements:_



[![ObjectProperty](../../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __actsFor__ (owl:ObjectProperty) The relation holding between any Agent, and a SocialAgent. In principle, a SocialAgent requires at least one PhysicalAgent in order to act, but this dependency can be 'delegated'; e.g. a university can be acted for by a department, which on its turm is acted for by physical agents. 
 [![](../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[actsFor](../Submissions/ActingFor/actsFor.md "Submissions:ActingFor/actsFor") page_
[![ObjectProperty](../../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __actsThrough__ (owl:ObjectProperty) The relation holding between a PhysicalAgent and a SocialAgent. In principle, a SocialAgent requires at least one PhysicalAgent in order to act, but this dependency can be 'delegated', e.g. a university can be acted for by a department, which is acted for by physical agents. 
 [![](../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[actsThrough](../Submissions/ActingFor/actsThrough.md "Submissions:ActingFor/actsThrough") page_
[![Class](../../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif.md "Class") __Agent__ (owl:Class) Any agentive Object , either physical (e.g. a whale, a robot, an oak), or social (e.g. a corporation, an institution, a community).
  



Additional comment: a computational agent can be considered as a PhysicalAgent that realizes a certain class of algorithms (that can be considered as instances of InformationObject) that allow to obtain some behaviors that are considered typical of agents in general. For an ontology of computational objects based on DOLCE see e.g. and [http://www.loa-cnr.it/COS/COS.owl](http://www.loa-cnr.it/COS/COS.owl "http://www.loa-cnr.it/COS/COS.owl"), and [http://www.loa-cnr.it/KCO/KCO.owl](http://www.loa-cnr.it/KCO/KCO.owl "http://www.loa-cnr.it/KCO/KCO.owl"). 



 [![](../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[Agent](../Submissions/ActingFor/Agent.md "Submissions:ActingFor/Agent") page_
[![Class](../../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif.md "Class") __SocialAgent__ (owl:Class) Any individual whose existence is granted simply by its social communicability and capability of action (through some PhysicalAgent). 
 [![](../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[SocialAgent](../Submissions/ActingFor/SocialAgent.md "Submissions:ActingFor/SocialAgent") page_
#  Additional information


#  Scenarios



__Scenarios about ActingFor__
No scenario is added to this Content OP.




#  Reviews



__Reviews about ActingFor__
There is no review about this proposal.
This revision (revision ID __10789__) takes in account the reviews: none


Other info at [evaluation tab](http://ontologydesignpatterns.org/wiki/index.php?title=Submissions:ActingFor&action=evaluation "http://ontologydesignpatterns.org/wiki/index.php?title=Submissions:ActingFor&action=evaluation")




  




#  Modeling issues



__Modeling issues about ActingFor__
There is no Modeling issue related to this proposal.




  




#  References


[Add a reference](index.php@title=Odp%253AAdd_reference&subject=../Submissions/ActingFor.md "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_reference&subject=Submissions%3AActingFor")


  






Retrieved from "[http://ontologydesignpatterns.org/wiki/Submissions:ActingFor](../Submissions/ActingFor.md)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [ProposedContentOP](../Category/ProposedContentOP.md "Category:ProposedContentOP")