[![](../images/thumb/b/b5/Certified.png/70px-Certified.png)](../Image/Certified.png.md "Certified.png") __This pattern has been certified.__
Related submission, with evaluation history, can be found __here__





#  Graphical representation


__Diagram__




[![Image:Description.jpg](../images/6/61/Description.jpg)](../Image/Description.jpg.md "Image:Description.jpg")




#  General description


  




#  Elements


_The __Description__ Content OP locally defines the following ontology elements:_




[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif.md "Class") __Description__ (owl:Class) A description represents a conceptualization. It can be thought also as a descriptive
context that defines concepts in order to see a relational context out of a set of data or observations.
For example, a Plan is a description of some actions to be executed by agents in a certain way, with
certain parameters; a diagnosis is a description that provides an interpretation to a set of observed
entities, etc. 



 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[Description](../Submissions/Description/Description.md "Submissions:Description/Description") page_

[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif.md "Class") __Concept__ (owl:Class) A __concept__ can be an idea, notion, role, or even a reified class, and is defined in a description.
Once defined, a concept can be used in other descriptions. 



 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[Concept](../Submissions/Description/Concept.md "Submissions:Description/Concept") page_

[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __is defined in__ (owl:ObjectProperty) A relation between a description and a concept, e.g. a workflow for a governmental
organization defines the role officer, or the Italian Traffic Law defines the role Vehicle. In order to be
used, a concept must be previously defined in another description. The  [defines](../Submissions/Description/defines.md "Submissions:Description/defines") object property is its inverse. 



 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[isDefinedIn](../Submissions/Description/isDefinedIn.md "Submissions:Description/isDefinedIn") page_

[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __is concept used in__ (owl:ObjectProperty) a more generic relation holding between a description and a concept.
The  [uses concept](../Submissions/Description/usesConcept.md "Submissions:Description/usesConcept") object property is its inverse. 



 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[isConceptUsedIn](../Submissions/Description/isConceptUsedIn.md "Submissions:Description/isConceptUsedIn") page_

[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __defines__ (owl:ObjectProperty) A relation between a  [Description](../Submissions/Description/Description.md "Submissions:Description/Description") and a  [Concept](../Submissions/Description/Concept.md "Submissions:Description/Concept"), e.g. a Workflow for a governmental Organization defines the Role 'officer', or 'the Italian Traffic Law defines the role Vehicle'.  [isDefinedIn](../Submissions/Description/isDefinedIn.md "Submissions:Description/isDefinedIn") is its inverse. 



 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[defines](../Submissions/Description/defines.md "Submissions:Description/defines") page_

[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __uses concept__ (owl:ObjectProperty) A generic relation holding between a  [Description](../Submissions/Description/Description.md "Submissions:Description/Description") and a  [Concept](../Submissions/Description/Concept.md "Submissions:Description/Concept"). In order to be used, a Concept must be previously  [defined in](../Submissions/Description/isDefinedIn.md "Submissions:Description/isDefinedIn") another Description. This last condition cannot be encoded for object properties in OWL. 



 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[usesConcept](../Submissions/Description/usesConcept.md "Submissions:Description/usesConcept") page_
#  Additional information


#  Scenarios



__Scenarios about Description__
No scenario is added to this Content OP.




#  Reviews



__Reviews about Description__
There is no review about this proposal.
This revision (revision ID __9087__) takes in account the reviews: none


Other info at [evaluation tab](http://ontologydesignpatterns.org/wiki/index.php?title=Submissions:Description&action=evaluation "http://ontologydesignpatterns.org/wiki/index.php?title=Submissions:Description&action=evaluation")




  




#  Modeling issues



__Modeling issues about Description__

  




#  References


[Add a reference](index.php@title=Odp%253AAdd_reference&subject=../Submissions/Description.md "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_reference&subject=Submissions%3ADescription")


  






Retrieved from "[http://ontologydesignpatterns.org/wiki/Submissions:Description](../Submissions/Description.md)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [ProposedContentOP](../Category/ProposedContentOP.md "Category:ProposedContentOP")