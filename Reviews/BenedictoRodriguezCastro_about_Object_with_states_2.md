[![](../images/thumb/2/29/Reviewer.png/48px-Reviewer.png)](../Image/Reviewer.png.md "Reviewer.png")
__[BenedictoRodriguezCastro](../User/BenedictoRodriguezCastro.md "User:BenedictoRodriguezCastro") about [Object with states](../Submissions/Object_with_states.md "Submissions:Object with states") (Revision ID: [with states?oldid=11667 11667](../Submissions/Object.md "http://ontologydesignpatterns.org/wiki/Submissions:Object"))__
Overall suggestion (score): 1 - needs minor revision




 __Review Summary:__ The pattern "Objects with States" (OWS) proposes a solution to the modeling scenario in which an object may go through a series of different states, and for each given state different restrictions and implications may apply. 
The proposed pattern addresses a very recurrent modeling scenario in real world Web applications and puts forward a generic solution, domain-independent with a promising potential for reusability. In terms of functionality, the pattern submitted addresses the targeted modeling scenario. On the other hand, in terms of description and documentation, there are some important aspects captured in the rest of this report that in my view have not been sufficiently documented and discussed.



Overall, I think this pattern fits very well the WOP workshop and can provide a very interesting topic of discussion among participants. I would recommend a rating of 1 ("weak accept" or "needs minor revision").
__Reviewer Confidence:__ The pattern is described in general terms and the solution is applicable and relevant to many domains. The assessment of the pattern requires a good understanding of OWL modeling idioms, especially those involved in the Value Partition pattern, but no expertise in a particular application domain. In that sense, in a scale from 1 to 5, where 1 is "no confidence" and 5 is "expert", for this particular pattern, I would rate my confidence as 5.
__Problems:__ See sections:
- "Relation to Other Patterns", 


- "Overall Understandability", 


- "Clear Relevance and Consequences", 


- "Clear Figures and Illustrations", and



- "Missing information".
__Community Relevance:__ The scenario described is very frequent in real world Web applications and makes the pattern very relevant to the WOP workshop and the Ontology Engineering community.
__Relation to Best Practices:__ The pattern can be seen as a best practice for the modeling scenario described.
__Reusability:__ The pattern is given in general terms and is not dependent on any particular domain. In this sense, the potential for reusability is very promising.
__Relations to Other Patterns:__ As the author points out, the "Objects with states" (OWS) pattern is related to the Value Partition (VP) pattern given that the latter is used to model part of the elements in the former. 
However, I believe that the relation between the two is stronger than the author states. In fact I believe that "Objects with states" could be seen as simply an extension of the VP pattern because the parallelism between the two goes beyond what it is discussed in the submission.


For example, consider the graphocal representation of the OWS pattern given in the submission and Figure 1 in the VP pattern introduced at: [http://www.w3.org/TR/swbp-specified-values/](http://www.w3.org/TR/swbp-specified-values/ "http://www.w3.org/TR/swbp-specified-values/")


The following functional equivalences between the elements of both patterns (where functional equivalences refers to elements that perform the same or analogous function) could be identified:


- The State class partition (and its 3 individuals) is analogous to the Health\_Value class partition (and its 3 individuals).


- The has\_state property is analogous to the has\_health\_status property.


- The Object class is analogous to the Person class.


- The ObjectStateA, -B, -C classes are analogous to the class Healty\_Person and to the hypothetical classes Medium\_Health\_Person, Poor\_Health\_Person respectively if the last two were to be declared in the VP partition (which in Figure 1 are not).


Up to this point the OWS pattern can be seen as an instantiation of the VP pattern for a particular modeling scenario. The novelty of the OWS, where it extends the VP pattern, comes from these additional requirements:


- The OWS pattern requires a subclass of Object (ObjectStateA, -B, -C) for every individual of type State, while the VP pattern does not.


- The Object class is the disjoint union of its subclasses (which can be seen also as a VP pattern in itself as per Figure 2 in [http://www.w3.org/TR/swbp-specified-values/](http://www.w3.org/TR/swbp-specified-values/ "http://www.w3.org/TR/swbp-specified-values/")). This characteristic is not required by the VP pattern (i.e. Person does not have to be the disjoint union of Healty\_Person, etc.).


- The additional properties p1, p2, p3, etc. introduced to characterize the implications of an object being in a given state.


- The cardinality constraints in all object properties.


Conversely, there is a key feature in the VP pattern that in the version of the OWS submitted is not present or discussed. That is:


- The class Healthy\_Person includes an owl:equivalentClass axiom that allows a standard DL-reasoner to classify all individuals of type Person whose value for has\_health\_status is good\_health as individuals of type Healthy\_Person as well.


- Analogous inferences would be possible for individuals of type Object. They could be automatically classified as individuals of the corresponding ObjectStateA, -B, -C class, if these classes were to follow an implementation analogous to Healthy\_Person (replacing the applicable rdfs:subClassOf axiom for a owl:equivalentClass).



I believe the comparative analysis above between the OWS pattern and the VP pattern is relevant and it will improve the clarity and potential reusability of the OWS pattern.
__Overall Understandability:__ The understandability of the pattern is acceptable but it can be highly improved as per comments in sections:
- "Relation to Other Patterns", 


- "Clear Relevance and Consequences", 


- "Clear Figures and Illustrations", and



- "Missing information".
__Clear Problem Description:__ The description of the problem is clear.
__Clear Relevance and Consequences:__ The relevance and consequences are not discussed. These two aspects could be addressed providing some background and overall outlook of how this object with states modeling scenario have been handled (if at all) prior to the proposed solution by the author. What were the main shortcomings of those previous approaches?
__Clear Figures and Illustrations:__ The graphical representation of the generic OWS pattern submitted is adequate. It captures the relevant elements that participate in the realization of the pattern.
However, consider also adding a graphical representation of a specific example that instantiates the pattern. The submission already provides a textual description of such specific example in the context of software defects, yet a graphical representation will illustrate how the generic elements of the pattern map to the elements in the example.



This is considered a good practice for the documentation of design patterns in general.
__Missing Information:__ Firstly, see sections:
- "Relation to Other Patterns", 


- "Overall Understandability", 


- "Clear Relevance and Consequences", 


- "Clear Figures and Illustrations", and



And one more consideration. A known use case is provided in the form of an alm-istack.owl file. Please, consider providing a textual description to highlight the main aspects of this particular known use case with respect to the proposed pattern. At a glance, it seems that the pattern is instantiated several times in the .owl use case provided. Consider describing these different instantiations and how the main generic elements have been populated.

_Posted:_ 2013/8/8 _Last modified:_ 2013/8/8



[All reviews](../Reviews/Main.md "Reviews:Main") | [Add a comment at the bottom of this page](index.php@title=Odp%253AAdd_comment&target=../Reviews/BenedictoRodriguezCastro_about_Object_with_states_2.md#New_comment "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_comment&target=Reviews:BenedictoRodriguezCastro_about_Object_with_states_2#New_comment")


Retrieved from "[http://ontologydesignpatterns.org/wiki/Reviews:BenedictoRodriguezCastro\_about\_Object\_with\_states\_2](../Reviews/BenedictoRodriguezCastro_about_Object_with_states_2.md)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [QCReview](../Category/QCReview.md "Category:QCReview")