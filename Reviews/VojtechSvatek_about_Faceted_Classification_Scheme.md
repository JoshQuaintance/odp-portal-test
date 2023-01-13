[![](../images/thumb/2/29/Reviewer.png/48px-Reviewer.png)](../Image/Reviewer.png "Reviewer.png")
__[VojtechSvatek](../User/VojtechSvatek "User:VojtechSvatek") about [Faceted Classification Scheme](../Submissions/Faceted_Classification_Scheme "Submissions:Faceted Classification Scheme") (Revision ID: [Classification Scheme?oldid=10104 10104](../Submissions/Faceted "http://ontologydesignpatterns.org/wiki/Submissions:Faceted"))__
Overall suggestion (score): 1 - needs minor revision




 __Review Summary:__ A pattern that relatively straightforwardly applies another (more fundamental) pattern submitted in parallel, Normalization. Useful however. Minor presentation issues to be fixed.
__Reviewer Confidence:__ The pattern is fairly generic and I feel confident to review it.
__Problems:__ I don't like the phrase 'class that represents a subset of the... class', which the author uses. More formally, we should say that the \*interpretation\* of one class is a subset of the \*interpretation\* of the other class (i.e. not of the class itself). Or, most simply (and preferably) in the OWL context, we can say that one class is subclass of another.
While the categories in a FCS are defined as mutually exclusive and exhaustive, the present example does not seem to fulfill this, in particular for the Brand Name and Scent facets, which can hardly be exhaustive.



As concerns mutual exclusivity: the proposal does not explicitly state that the object properties representing the facets (such as hasAgent) have to be functional. Why?
__Community Relevance:__ Pretty relevant.
__Relation to Best Practices:__ Yes, I would see this pattern as best practice in the given context.
__Reusability:__ Relatively high. However, it would be worth considering explicitly extending the pattern to systems with \*hierarchical\* facets.
__Relations to Other Patterns:__ This (or, the Normalization pattern) actually seems to be a reflection of the construct proposed by A. Rector years ago, as the author (somewhat tacitly) acknowledges.
__Overall Understandability:__ Yes - the description is perhaps oversophisticated for a generic modeller; however, this is probably due to adaptation to the mindset of specialists in faceted systems, for which the pattern is intended.
__Clear Problem Description:__ Yes, the problem is sufficiently elaborated.
__Clear Relevance and Consequences:__ Pretty relevant; the consequences are sketched but could be elaborated more.
__Clear Figures and Illustrations:__ A minor issue: while the diagram of the Normalization pattern shows the class hierarchy before the property hierarchy, in the example it is the other way around.
__Missing Information:__ Especially that on possible functionality of the object properties, see above.

_Posted:_ 2010/9/17 _Last modified:_ 2010/9/17



[All reviews](../Reviews/Main "Reviews:Main") | [Add a comment at the bottom of this page](index.php@title=Odp%253AAdd_comment&target=../Reviews/VojtechSvatek_about_Faceted_Classification_Scheme#New_comment "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_comment&target=Reviews:VojtechSvatek_about_Faceted_Classification_Scheme#New_comment")


Retrieved from "[http://ontologydesignpatterns.org/wiki/Reviews:VojtechSvatek\_about\_Faceted\_Classification\_Scheme](../Reviews/VojtechSvatek_about_Faceted_Classification_Scheme)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [QCReview](../Category/QCReview "Category:QCReview")