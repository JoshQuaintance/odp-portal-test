[![](../images/thumb/2/29/Reviewer.png/48px-Reviewer.png)](../Image/Reviewer.png.md "Reviewer.png")
__[OlafNoppens](../User/OlafNoppens.md "User:OlafNoppens") about [Literal Reification](../Submissions/Literal_Reification.md "Submissions:Literal Reification") (Revision ID: [Reification?oldid=10062 10062](../Submissions/Literal.md "http://ontologydesignpatterns.org/wiki/Submissions:Literal"))__
Overall suggestion (score): 2 - accept for certification




 __Review Summary:__ The pattern states how to express reification of literal values in OWL by introducing an intermediate individual (type of Literal) which is connected (via hasLiteralValue) to a blank literal value, or via hasSameLiteralValue to another intermediate individual.
I have two minor remarks (which depends on each other):


(1) Literal is a subclass of (= 1 hasLiteralValue). I was wondering whether one could define literal equivalent to (= 1 hasLiteralValue or = 1 hasSameLiteralValue). The idea is that a literal has always either a literal value directly or indirectly (via hasSameLiteralValue)



(2)SWRL rules are used (in that sense it would also be valid if Literal is defined equivalent to = 1 hasLiteralValue because the SWRL rules guarantee this behaviour). I suggest to add a remark to the description and also to the diagram. Because the application of the pattern assumes SWRL + OWL.
__Reviewer Confidence:__ high
__Problems:__ 
__Community Relevance:__ high
__Relation to Best Practices:__ 
__Reusability:__ high
__Relations to Other Patterns:__ 
__Overall Understandability:__ good
__Clear Problem Description:__ good
__Clear Relevance and Consequences:__ good
__Clear Figures and Illustrations:__ good - I suggest as mentioned above that the desription and the figures make a reference to rules / SWRL
__Missing Information:__ 

_Posted:_ 2010/9/16 _Last modified:_ 2010/9/16



[All reviews](../Reviews/Main.md "Reviews:Main") | [Add a comment at the bottom of this page](index.php@title=Odp%253AAdd_comment&target=../Reviews/OlafNoppens_about_Literal_Reification.md#New_comment "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_comment&target=Reviews:OlafNoppens_about_Literal_Reification#New_comment")


Retrieved from "[http://ontologydesignpatterns.org/wiki/Reviews:OlafNoppens\_about\_Literal\_Reification](../Reviews/OlafNoppens_about_Literal_Reification.md)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [QCReview](../Category/QCReview.md "Category:QCReview")