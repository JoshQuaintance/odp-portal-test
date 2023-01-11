[![](../images/thumb/b/b5/Certified.png/70px-Certified.png)](../Image/Certified.png.md "Certified.png") __This pattern has been certified.__
Related submission, with evaluation history, can be found __here__





#  Graphical representation


__Diagram__
_(this article has no graphical representation)_



#  General description


  




#  Elements


_The __InformationObjectsAndRepresentationLanguages__ Content OP locally defines the following ontology elements:_



[![ObjectProperty](../../../../../../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __conceptualizes__ (owl:ObjectProperty) A relation stating that an Agent is internally representing a SocialObject . E.g., 'John believes in the conspiracy theory'; 'Niels Bohr created the solar-system metaphor for the atomic theory'; 'Jacques assumes all swans are white'; 'the task force members share the attack plan'. 
 [![](../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[conceptualizes](../Submissions/InformationObjectsAndRepresentationLanguages/conceptualizes.md "Submissions:InformationObjectsAndRepresentationLanguages/conceptualizes") page_
[![ObjectProperty](../../../../../../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __formallyRepresents__ (owl:ObjectProperty) The relation between formal expressions, and anything that they are supposed to represent.
E.g., 'the predicate 'MariachiInTijuana' formallyRepresents the dul:Collection of all mariachis in Tijuana'; 'the equivalence relation '<=>' formallyRepresents the concept of two entities having the same properties'.


Notice that formal expressions are formally interpreted by instances of dul:FormalEntity 



 [![](../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[formallyRepresents](../Submissions/InformationObjectsAndRepresentationLanguages/formallyRepresents.md "Submissions:InformationObjectsAndRepresentationLanguages/formallyRepresents") page_
[![ObjectProperty](../../../../../../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __hasRepresentationLanguage__ (owl:ObjectProperty) 
 [![](../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[hasRepresentationLanguage](../Submissions/InformationObjectsAndRepresentationLanguages/hasRepresentationLanguage.md "Submissions:InformationObjectsAndRepresentationLanguages/hasRepresentationLanguage") page_
[![ObjectProperty](../../../../../../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __isConceptualizedBy__ (owl:ObjectProperty) A relation stating that an Agent is internally representing a Description . E.g., 'John believes in the conspiracy theory'; 'Niels Bohr created a solar-system metaphor for his atomic theory'; 'Jacques assumes all swans are white'; 'the task force shares the attack plan'. 
 [![](../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[isConceptualizedBy](../Submissions/InformationObjectsAndRepresentationLanguages/isConceptualizedBy.md "Submissions:InformationObjectsAndRepresentationLanguages/isConceptualizedBy") page_
[![ObjectProperty](../../../../../../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __isFormallyRepresentedIn__ (owl:ObjectProperty) The relation between formal expressions, and anything that they are supposed to represent.
E.g., 'the predicate 'MariachiInTijuana' formallyRepresents the dul:Collection of all mariachis in Tijuana'; 'the equivalence relation '<=>' formallyRepresents the concept of two entities having the same properties'.


Notice that formal expressions are formally interpreted by instances of dul:FormalEntity 



 [![](../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[isFormallyRepresentedIn](../Submissions/InformationObjectsAndRepresentationLanguages/isFormallyRepresentedIn.md "Submissions:InformationObjectsAndRepresentationLanguages/isFormallyRepresentedIn") page_
[![ObjectProperty](../../../../../../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __isRepresentationLanguageOf__ (owl:ObjectProperty) 
 [![](../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[isRepresentationLanguageOf](../Submissions/InformationObjectsAndRepresentationLanguages/isRepresentationLanguageOf.md "Submissions:InformationObjectsAndRepresentationLanguages/isRepresentationLanguageOf") page_
[![Class](../../../../../../../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif.md "Class") __FormalExpression__ (owl:Class) Any information object represented in a FormalLanguage, usually having a formal interpretation by a dul:FormalEntity, and used to formally represent any Entity 
 [![](../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[FormalExpression](../Submissions/InformationObjectsAndRepresentationLanguages/FormalExpression.md "Submissions:InformationObjectsAndRepresentationLanguages/FormalExpression") page_
[![Class](../../../../../../../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif.md "Class") __FormalLanguage__ (owl:Class) A formal language, created by some human, with a fixed grammar, and usually with an explicit formal semantics (i.e. its elements have an interpretation wrt to formal entities such as sets, categories, etc.). 
 [![](../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[FormalLanguage](../Submissions/InformationObjectsAndRepresentationLanguages/FormalLanguage.md "Submissions:InformationObjectsAndRepresentationLanguages/FormalLanguage") page_
[![Class](../../../../../../../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif.md "Class") __IconicLanguage__ (owl:Class) A language made up of graphical elements. It can be natural, artificial, and even formal. 
 [![](../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[IconicLanguage](../Submissions/InformationObjectsAndRepresentationLanguages/IconicLanguage.md "Submissions:InformationObjectsAndRepresentationLanguages/IconicLanguage") page_
[![Class](../../../../../../../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif.md "Class") __IconicObject__ (owl:Class) An information object represented in an IconicLanguage 
 [![](../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[IconicObject](../Submissions/InformationObjectsAndRepresentationLanguages/IconicObject.md "Submissions:InformationObjectsAndRepresentationLanguages/IconicObject") page_
[![Class](../../../../../../../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif.md "Class") __Language__ (owl:Class) A natural or artificial language, provided with an alphabet (or vocabulary) and combinatorial rules. In the case of natural languages, their components are 'temporary' and 'reconstructed' out of actual usage. For example, a grammar for a natural language has the status of a theory for that language, and alternative ones can exist (e.g. generative vs. construction grammars).
Another distinction, between the general (systemic) rules for a language, and the local (contextual) rules for e.g. a certain context, speaker, place, etc., can be made separately.


The most comprehensive classification of languages ha probably been made by Umberto Eco, based on the production modes of the 'signs' that are represented in a certain language. It uses several semiotic dimensions, and will be modeled in a forthcoming ontology. 



 [![](../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[Language](../Submissions/InformationObjectsAndRepresentationLanguages/Language.md "Submissions:InformationObjectsAndRepresentationLanguages/Language") page_
[![Class](../../../../../../../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif.md "Class") __LinguisticObject__ (owl:Class) An information object represented in a NaturalLanguage 
 [![](../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[LinguisticObject](../Submissions/InformationObjectsAndRepresentationLanguages/LinguisticObject.md "Submissions:InformationObjectsAndRepresentationLanguages/LinguisticObject") page_
[![Class](../../../../../../../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif.md "Class") __NaturalLanguage__ (owl:Class) A natural language, evolved and used in a community across time.
Natural languages components are 'temporary' and 'reconstructed' out of actual usage. For example, a grammar for a (part of a) natural language has the status of a theory for that language, but alternative ones can exist (e.g. generative vs. construction grammars). 



 [![](../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[NaturalLanguage](../Submissions/InformationObjectsAndRepresentationLanguages/NaturalLanguage.md "Submissions:InformationObjectsAndRepresentationLanguages/NaturalLanguage") page_
#  Additional information


#  Scenarios



__Scenarios about InformationObjectsAndRepresentationLanguages__
No scenario is added to this Content OP.




#  Reviews



__Reviews about InformationObjectsAndRepresentationLanguages__
There is no review about this proposal.
This revision (revision ID __9094__) takes in account the reviews: none


Other info at [evaluation tab](http://ontologydesignpatterns.org/wiki/index.php?title=Submissions:InformationObjectsAndRepresentationLanguages&action=evaluation "http://ontologydesignpatterns.org/wiki/index.php?title=Submissions:InformationObjectsAndRepresentationLanguages&action=evaluation")




  




#  Modeling issues



__Modeling issues about InformationObjectsAndRepresentationLanguages__
There is no Modeling issue related to this proposal.




  




#  References


[Add a reference](index.php@title=Odp%253AAdd_reference&subject=../Submissions/InformationObjectsAndRepresentationLanguages.md "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_reference&subject=Submissions%3AInformationObjectsAndRepresentationLanguages")


  






Retrieved from "[http://ontologydesignpatterns.org/wiki/Submissions:InformationObjectsAndRepresentationLanguages](../Submissions/InformationObjectsAndRepresentationLanguages.md)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [ProposedContentOP](../Category/ProposedContentOP.md "Category:ProposedContentOP")