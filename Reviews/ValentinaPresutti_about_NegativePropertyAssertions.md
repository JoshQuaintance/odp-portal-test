[![](../images/thumb/2/29/Reviewer.png/48px-Reviewer.png)](../Image/Reviewer.png.md "Reviewer.png")
__[ValentinaPresutti](../User/ValentinaPresutti.md "User:ValentinaPresutti") about [NegativePropertyAssertions](../Submissions/NegativePropertyAssertions.md "Submissions:NegativePropertyAssertions") (Revision ID: [5769](../Submissions/NegativePropertyAssertions@oldid=5769.md "http://ontologydesignpatterns.org/wiki/Submissions:NegativePropertyAssertions?oldid=5769"))__
Overall suggestion (score): 1 - needs minor revision




 __Review Summary:__ This submission has the aim of solving the problem of expressing negative property assertions (NPA) in OWL 1. I have to admit I never consider this problem before, and it can be interesting to identify a way to express NPA in OWL 1, that has not such a primitive. 
I think it could be interesting to have this pattern at the workshop but it is very badly described at the moment, it needs major revisions.
My main concerns can be summarized as follows: 



* are there use case for this? and which are? I can imagine it would be useful to identify such a logical structure in OWL 1 ontologies in order to allow a conversion to OWL 2 that replace them with NPAs.
* the author claims the OWL 1 logical expression is equivalent to the NPA provided by OWL 2. If they are equivalent, I would expect a formal proof, if the OWL 1 expression approximates the OLW 2 NPA, then I would expect at least a detailed explanation of what are the consequences of this approximation. In other words, the submission is not accurate
* the syntax used is not introduced, neither with a simple reference
* the description of the problem is to vague and with no use case,s cenarios
* the pattern is not detailed enough in all its part


__Reviewer Confidence:__ My confidence is medium/good with respect to all aspects. I didn't consider the problem before, but had a look at the OWL 2 spec and believe I understood the logical problem.
__Problems:__ I think that the two logical expressions are not equivalent. To assert that "i1 is not in the class of things that have value i2 for property prop" is a bit different from asserting that "i2 has not the value i2 for property prop", because in the latter case the assertion is explicit. I think that this argument should be clarified and exhaustively discussed in the pattern description. 
It seems to me that there is a useless bracket
__Community Relevance:__ medium
__Relation to Best Practices:__ 
__Reusability:__ The pattern is general as it is a logical pattern. Btw its exposition is poor and clarity is not so good. Also no documentation and use cases are provided, hence it would be not straightforward to reuse it.
__Relations to Other Patterns:__ Not in my knowledge.
__Overall Understandability:__ poor
__Clear Problem Description:__ poor
__Clear Relevance and Consequences:__ poor
__Clear Figures and Illustrations:__ poor
__Missing Information:__ figures, illustration, use cases, scenarios, consequences, proof.

_Posted:_ 2009/9/9 _Last modified:_ 2009/9/9



[All reviews](../Reviews/Main.md "Reviews:Main") | [Add a comment at the bottom of this page](index.php@title=Odp%253AAdd_comment&target=../Reviews/ValentinaPresutti_about_NegativePropertyAssertions.md#New_comment "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_comment&target=Reviews:ValentinaPresutti_about_NegativePropertyAssertions#New_comment")


Retrieved from "[http://ontologydesignpatterns.org/wiki/Reviews:ValentinaPresutti\_about\_NegativePropertyAssertions](../Reviews/ValentinaPresutti_about_NegativePropertyAssertions.md)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [QCReview](../Category/QCReview.md "Category:QCReview")