[![](../images/thumb/2/29/Reviewer.png/48px-Reviewer.png)](../Image/Reviewer.png "Reviewer.png")
__[AlessandroAdamou](../User/AlessandroAdamou "User:AlessandroAdamou") about [Object with states](../Submissions/Object_with_states "Submissions:Object with states") (Revision ID: [with states?oldid=11650 11650](../Submissions/Object "http://ontologydesignpatterns.org/wiki/Submissions:Object"))__
Overall suggestion (score): 1 - needs minor revision




 __Review Summary:__ The pattern provides a reasonable solution to one of the core issues in ontology modeling, but it should not be standalone and its ontology should be generalised.
__Reviewer Confidence:__ ODP: expert
Ontology engineering: high



State machines : fair
__Problems:__ \* the pattern has no dependencies, whereas it seems to have strong ties with catalogued patterns such as Situation (of which it seems to be a suitable extension) and Parameter;
* the partitioning of states, objects with states, and their resulting properties, into exactly three items is hardwired in the ontology itself. As it is used to exemplify its usage, it should not appear in the core ontology.


__Community Relevance:__ The ODP addresses a horizontal problem in ontology modeling, although by ruling out or underspecifying spatial and temporal contexts of states, it restricts more than it should.
__Relation to Best Practices:__ Can be effectively applied to state machine modeling - for comparison see Dolog's FSM ontology, doc at [http://people.cs.aau.dk/~dolog/fsm/](http://people.cs.aau.dk/~dolog/fsm/ "http://people.cs.aau.dk/~dolog/fsm/")
__Reusability:__ Fair - highly reusable if we assume an ontology to model shapshot data, less reusable for modeling historical data.
__Relations to Other Patterns:__ IMO it should depend on Situation (as it seems to be specialising it) and Bag (for abstracting over the partitioning of state objects in exactly three subclasses)
__Overall Understandability:__ The ontology and its members are annotated appropriately.
__Clear Problem Description:__ Competency questions are not formulated according to standards, but the intent and solution description are reasonably clear.
__Clear Relevance and Consequences:__ The requirement of modeling states as individuals is a significant example of conformance to best practices.
The current ODP has a strict limitation to tripartite states - if this is not relaxed, it should be mentioned in the consequences.
__Clear Figures and Illustrations:__ Figure is clear, but if possible please use arrows with no fill for subclasses.
As it is meant to represent a usage schema, it is okay to retain the tripartition of Object and State in the figure. Maybe it could be made as State1, State2, ... StateN and the like
__Missing Information:__ The link to the example usage in Known Usage should appear in the field "Examples (OWL files)".
Other than that, missing information is a consequence of the pattern not having been related to other ODPs.

_Posted:_ 2013/8/7 _Last modified:_ 2013/8/7



[All reviews](../Reviews/Main "Reviews:Main") | [Add a comment at the bottom of this page](index.php@title=Odp%253AAdd_comment&target=../Reviews/AlessandroAdamou_about_Object_with_states#New_comment "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_comment&target=Reviews:AlessandroAdamou_about_Object_with_states#New_comment")


Retrieved from "[http://ontologydesignpatterns.org/wiki/Reviews:AlessandroAdamou\_about\_Object\_with\_states](../Reviews/AlessandroAdamou_about_Object_with_states)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [QCReview](../Category/QCReview "Category:QCReview")