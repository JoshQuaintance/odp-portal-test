[![](../images/thumb/2/29/Reviewer.png/48px-Reviewer.png)](../Image/Reviewer.png "Reviewer.png")
__[RinkeHoekstra](../User/RinkeHoekstra "User:RinkeHoekstra") about [Object with states](../Submissions/Object_with_states "Submissions:Object with states") (Revision ID: [with states?oldid=11667 11667](../Submissions/Object "http://ontologydesignpatterns.org/wiki/Submissions:Object"))__
Overall suggestion (score): 0 - needs major revision




 __Review Summary:__ The design pattern is intended to allow the representation of objects with states. To this end, the author proposes to define objects as classes with certain properties, and link them to separate individuals that represent the state of the object using a 'hasState' property.
The author does not really discuss related work, most prominently e.g. the perdurants of the DOLCE ontology. Also, I do not think the solution is satisfactory, or at least it is not very generalizable nor very strictly defined. Detailed comments below:



* It seems ontologically strange to define 'objects' as classes, whereas the states are individuals associated to \*instances\* of those object classes using the 'hasState' property. A more pragmatic solution would be to decide that all individuals of type 'Object' are also states. One can then individuate an object through time (i.e. through all its states) by chaining these states together using a property of choice. Another option would be to consider all states that are instances of a certain object class to be states of the same object. The object class then represents the object as it exists through time (perhaps this is closest to the currently proposed pattern)
* Secondly, it could be argued that there should not be a strict requirement that the states of an object are distinct individuals. For instance, I can be both married and brown-haired at the same time. Distinct individuals is a design decision that the author should argue for explicitly.
* The design pattern does not ensure that individual states are only the state of a \*single\* object. I.e. the has-state property should be inverse functional.


__Reviewer Confidence:__ fairly high
__Problems:__ \* It seems ontologically strange to define 'objects' as classes, whereas the states are individuals associated to \*instances\* of those object classes using the 'hasState' property. A more pragmatic solution would be to decide that all individuals of type 'Object' are also states. One can then individuate an object through time (i.e. through all its states) by chaining these states together using a property of choice. Another option would be to consider all states that are instances of a certain object class to be states of the same object. The object class then represents the object as it exists through time (perhaps this is closest to the currently proposed pattern) 
* Secondly, it could be argued that there should not be a strict requirement that the states of an object are distinct individuals. For instance, I can be both married and brown-haired at the same time. Distinct individuals is a design decision that the author should argue for explicitly.
* The design pattern does not ensure that individual states are only the state of a \*single\* object. I.e. the has-state property should be inverse functional.


__Community Relevance:__ The pattern, and its subject, is very relevant for the community as it is a very often occurring pattern in ontology engineering and modeling in general.
__Relation to Best Practices:__ The pattern does not really take into account the best practices around this subject. Objects and their states are discussed at length in the literature (though mostly philosophically inspired). It is fair enough that the author takes a pragmatic approach (which is laudable), but consulting related work would most likely improve the quality of the pattern.
__Reusability:__ The pattern is reusable.
__Relations to Other Patterns:__ 
__Overall Understandability:__ The pattern is understandable (the problem it tries to solve is clear), but it is formally underspecified.
__Clear Problem Description:__ The problem is clear
__Clear Relevance and Consequences:__ Consequences are not really made clear in the description. For instance, the assumption that states are distinct individuals is not sufficiently motivated nor discussed.
__Clear Figures and Illustrations:__ Yes
__Missing Information:__ A discussion of design decisions with reference to the literature would really help engineers in choosing this pattern.

_Posted:_ 2013/8/12 _Last modified:_ 2013/8/12



[All reviews](../Reviews/Main "Reviews:Main") | [Add a comment at the bottom of this page](index.php@title=Odp%253AAdd_comment&target=../Reviews/RinkeHoekstra_about_Object_with_states#New_comment "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_comment&target=Reviews:RinkeHoekstra_about_Object_with_states#New_comment")


Retrieved from "[http://ontologydesignpatterns.org/wiki/Reviews:RinkeHoekstra\_about\_Object\_with\_states](../Reviews/RinkeHoekstra_about_Object_with_states)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [QCReview](../Category/QCReview "Category:QCReview")