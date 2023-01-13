[![](../images/thumb/b/b5/Certified.png/70px-Certified.png)](../Image/Certified.png.md "Certified.png") __This pattern has been certified.__
Related submission, with evaluation history, can be found __here__





__Diagram__
_(this article has no graphical representation)_



#  General description


  




#  Elements


_The __Persons__ Content OP locally defines the following ontology elements:_



[![ObjectProperty](../../../../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __actsFor__ (owl:ObjectProperty) The relation holding between any Agent, and a SocialPerson. In principle, a SocialPerson requires at least one NaturalPerson in order to act, but this dependency can be 'delegated'; e.g. a university can be acted for by a department, which on its turm is acted for by natural persons. 
 [![](../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[actsFor](../Submissions/Persons/actsFor.md "Submissions:Persons/actsFor") page_
[![ObjectProperty](../../../../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __actsThrough__ (owl:ObjectProperty) The relation holding between any Agent, and a SocialPerson. In principle, a SocialPerson requires at least one NaturalPerson in order to act, but this dependency can be 'delegated'; e.g. a university can be acted for by a department, which on its turm is acted for by natural persons. 
 [![](../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[actsThrough](../Submissions/Persons/actsThrough.md "Submissions:Persons/actsThrough") page_
[![ObjectProperty](../../../../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __introduces__ (owl:ObjectProperty) A relation between a Description and a SocialPerson, e.g. a Constitutional Charter that introduces the SocialPerson 'PresidentOfRepublic'. 
 [![](../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[introduces](../Submissions/Persons/introduces.md "Submissions:Persons/introduces") page_
[![ObjectProperty](../../../../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __isIntroducedBy__ (owl:ObjectProperty) A relation between a Description and a SocialPerson, e.g. a Constitutional Charter that introduces the SocialPerson 'PresidentOfRepublic'. 
 [![](../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[isIntroducedBy](../Submissions/Persons/isIntroducedBy.md "Submissions:Persons/isIntroducedBy") page_
[![Class](../../../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif.md "Class") __NaturalPerson__ (owl:Class) A Person in the physical commonsense intuition: 'have you seen that person walking down the street?' 
 [![](../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[NaturalPerson](../Submissions/Persons/NaturalPerson.md "Submissions:Persons/NaturalPerson") page_
[![Class](../../../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif.md "Class") __Person__ (owl:Class) Persons in commonsense intuition, which does not apparently distinguish between either natural or social persons. 
 [![](../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[Person](../Submissions/Persons/Person.md "Submissions:Persons/Person") page_
[![Class](../../../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif.md "Class") __SocialPerson__ (owl:Class) A Person that needs the existence of a specific NaturalPerson in order to act (but the lifetime of the NaturalPerson has only to overlap that of the SocialPerson). The NaturalPerson through which it acts can be also indirectly related, e.g. an organization that acts through another organization, which actsThrough one or more NaturalPerson(s). 
 [![](../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[SocialPerson](../Submissions/Persons/SocialPerson.md "Submissions:Persons/SocialPerson") page_
  




#  Scenarios



__Scenarios about Persons__
No scenario is added to this Content OP.




#  Reviews



__Reviews about Persons__
There is no review about this proposal.
This revision (revision ID __8255__) takes in account the reviews: none


Other info at [evaluation tab](http://ontologydesignpatterns.org/wiki/index.php?title=Submissions:Persons&action=evaluation "http://ontologydesignpatterns.org/wiki/index.php?title=Submissions:Persons&action=evaluation")




#  Modeling issues



__Modeling issues about Persons__
There is no Modeling issue related to this proposal.






Retrieved from "[http://ontologydesignpatterns.org/wiki/Submissions:Persons](../Submissions/Persons.md)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [ProposedContentOP](../Category/ProposedContentOP.md "Category:ProposedContentOP")