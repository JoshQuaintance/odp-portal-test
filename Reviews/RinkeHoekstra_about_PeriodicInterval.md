[![](../images/thumb/2/29/Reviewer.png/48px-Reviewer.png)](../Image/Reviewer.png.md "Reviewer.png")
__[RinkeHoekstra](../User/RinkeHoekstra.md "User:RinkeHoekstra") about [PeriodicInterval](../Submissions/PeriodicInterval.md "Submissions:PeriodicInterval") (Revision ID: [11152](../Submissions/PeriodicInterval@oldid=11152.md "http://ontologydesignpatterns.org/wiki/Submissions:PeriodicInterval?oldid=11152"))__
Overall suggestion (score): 0 - needs major revision




 __Review Summary:__ The pattern for periodic intervals is highly relevant in many scenarios. It is a useful extension of the OWL Time ontology. It adequately imports the CP annotation schema, but does not really provide any documentation 
However, the pattern is too simplistic in its current form. In a way, the current definition can be read as a recipe for instantiating the sub intervals. This is done via a single object property (hasIntervalDurationPerPeriod), but could have been represented in OWL as restrictions on the PeriodicInterval class itself, e.g. it could be defined as a class with only subintervals of a particular length. The authors could spend some time thinking of how to augment their definition to make it more expressive (e.g. how to make sure the subintervals do not overlap)



Furthermore, the pattern does not adequately restrict the class, it only defines domain and range of two new properties. A PeriodicInterval should at least have two subintervals and a period that separates them.
__Reviewer Confidence:__ High
__Problems:__ The pattern is overly simplistic (see summary)
__Community Relevance:__ High
__Relation to Best Practices:__ The pattern does not present a best practice
__Reusability:__ High
__Relations to Other Patterns:__ Many in the category Time, but in particular [Submissions:TimeInterval](../Submissions/TimeInterval.md "Submissions:TimeInterval") and [Submissions:Sequence](../Submissions/Sequence.md "Submissions:Sequence")
__Overall Understandability:__ Ok
__Clear Problem Description:__ Ok
__Clear Relevance and Consequences:__ Ok
__Clear Figures and Illustrations:__ Yes
__Missing Information:__ 

_Posted:_ 2012/8/21 _Last modified:_ 2012/8/21



[All reviews](../Reviews/Main.md "Reviews:Main") | [Add a comment at the bottom of this page](index.php@title=Odp%253AAdd_comment&target=../Reviews/RinkeHoekstra_about_PeriodicInterval.md#New_comment "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_comment&target=Reviews:RinkeHoekstra_about_PeriodicInterval#New_comment")


Retrieved from "[http://ontologydesignpatterns.org/wiki/Reviews:RinkeHoekstra\_about\_PeriodicInterval](../Reviews/RinkeHoekstra_about_PeriodicInterval.md)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [QCReview](../Category/QCReview.md "Category:QCReview")