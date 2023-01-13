[![](../images/thumb/2/29/Reviewer.png/48px-Reviewer.png)](../Image/Reviewer.png "Reviewer.png")
__[AlessandroAdamou](../User/AlessandroAdamou "User:AlessandroAdamou") about [Inverse n-ary relationship](../Submissions/Inverse_n-ary_relationship "Submissions:Inverse n-ary relationship") (Revision ID: [n-ary relationship?oldid=10101 10101](../Submissions/Inverse "http://ontologydesignpatterns.org/wiki/Submissions:Inverse"))__
Overall suggestion (score): 0 - needs major revision




 __Review Summary:__ The authors propose an extension to the N-ary relationship pattern where two major participants are short-circuited by means of an inverse property pair.  

While the intent is admirable (though it requires a clearer explanation), such a solution does not seem to take into account possible in-house solutions provided by the ontology language.
__Reviewer Confidence:__ Expert in ODPs, fairly competent in Description Logics and OWL(2) constructs.
__Problems:__ The pattern naming can be confusing, since it somehow looks more like a "bridged" or "short-circuited" n-ary relationship.  

In OWL2, there should be some consideration for property chaining, which could link the properties that hold between the main actors and the N-ary relationship class. This would partly offer an in-house solution to the issue addressed as well as an elegant way to link relationships with one another, though it would probably require the intervention of reasoners.
__Community Relevance:__ It would be useful to discuss in a workshop to what extent this proposal qualifies as a pattern.
__Relation to Best Practices:__ Is this proposal supposed to provide an override for the practice of providing inverse property pairs for relationships? According to the figures, inverses appear to be superfluous for "minor" participants to the relationship.
__Reusability:__ Comparable to the n-ary relationship pattern.
__Relations to Other Patterns:__ This proposal extends the N-ary relationship pattern for particular yet not infrequent cases where two of the actors involved play a major role in the n-ary relationship.
__Overall Understandability:__ Flawed. Could raise the score by one entire point if properly reformulated (see below).  

Watch out for a few typos : "patter" and "exits" in the motivation, "querys" in the problem example, "taht" in the consequences...
__Clear Problem Description:__ The problem is better described in the example than in the motivation. The three reasons for using this pattern are not very clear at all: what does it mean that a relationship "is really amongst" several things and that it "really needs" a further argument? Are these three conditions supposed to hold altogether? It looks like that.  

On the other hand, the aim to speed up frequent queries is comprehensible.
__Clear Relevance and Consequences:__ Clear if we don't take into account that the "bridge" property pair does not show a connection to those between the main participants and the n-ary relationship class.
__Clear Figures and Illustrations:__ The figures seem to show that some inverse properties may be unneeded for what are considered as additional arguments. Also, the abstract version should be made a little more "general", by pointing out that the minor relations are in an arbitrary [1..n] amount.
__Missing Information:__ 

_Posted:_ 2010/9/16 _Last modified:_ 2010/9/16



[All reviews](../Reviews/Main "Reviews:Main") | [Add a comment at the bottom of this page](index.php@title=Odp%253AAdd_comment&target=../Reviews/AlessandroAdamou_about_Inverse_n-ary_relationship#New_comment "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_comment&target=Reviews:AlessandroAdamou_about_Inverse_n-ary_relationship#New_comment")


Retrieved from "[http://ontologydesignpatterns.org/wiki/Reviews:AlessandroAdamou\_about\_Inverse\_n-ary\_relationship](../Reviews/AlessandroAdamou_about_Inverse_n-ary_relationship)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [QCReview](../Category/QCReview "Category:QCReview")