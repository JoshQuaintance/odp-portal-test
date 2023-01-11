[![](../images/thumb/2/29/Reviewer.png/48px-Reviewer.png)](../Image/Reviewer.png.md "Reviewer.png")
__[AlessandroAdamou](../User/AlessandroAdamou.md "User:AlessandroAdamou") about [Symmetric n-ary relationship](../Submissions/Symmetric_n-ary_relationship.md "Submissions:Symmetric n-ary relationship") (Revision ID: [n-ary relationship?oldid=10106 10106](../Submissions/Symmetric.md "http://ontologydesignpatterns.org/wiki/Submissions:Symmetric"))__
Overall suggestion (score): 0 - needs major revision




 __Review Summary:__ While the problem this pattern tries to address cannot go unnoticed in OWL modelling, little explanation is provided as to how it distinguishes from built-in symmetric properties in OWL. As it is, the proposed pattern seems rather awkward for production use, and its naming can be misleading.
__Reviewer Confidence:__ Expert in ODPs, fairly competent in Description Logics and OWL(2) constructs.
__Problems:__ The pattern as it is conceived seems to be trying to cover all with a short blanket. While it does eliminate the redundancy of providing property pairs, it lends itself to the risk of an uncontrolled growth of n-ary relationship subclasses. What happens if we need to determine the distances between lots of places? Would this result in a new class for each distinguished value for a distance between to places?
  




Talking about "n-ary" symmetry sounds a bit confusing, as symmetry is commonly supposed to hold for binary relationships. The way the pattern is built, "binary" instead of "n-ary" could perhaps suit better.
__Community Relevance:__ Unquestionably relevant.
__Relation to Best Practices:__ 
__Reusability:__ Fair, provided that some more focused naming is given in order to appeal to more "casual" ontology engineers, but it is only better understood along with the other supplied figure for the distance example.
__Relations to Other Patterns:__ Despite being a special case of usage for the N-ary Relationship pattern, it seems like a bit of an overkill to employ for solving the given problem.
__Overall Understandability:__ Fairly comprehensible, though it could use a less misleading name.
__Clear Problem Description:__ From a purely OWL perspective, this problem seems to come into play when datatype properties are involved, while for object properties it should suffice to set the symmetric flag. This distinction should be pointed out, otherwise an explanation why it is not pertinent to the datatype/object property pair should be given.
__Clear Relevance and Consequences:__ As stated earlier, this proposal seems to be generating side effects with rspect to redundancy. If the authors can rule out these side effects, they should make a clearer statement about them.
__Clear Figures and Illustrations:__ The supplied figure is clear enough for knowledgeable N-ary relationship pattern users.
__Missing Information:__ 

_Posted:_ 2010/9/16 _Last modified:_ 2010/9/16



[All reviews](../Reviews/Main.md "Reviews:Main") | [Add a comment at the bottom of this page](index.php@title=Odp%253AAdd_comment&target=../Reviews/AlessandroAdamou_about_Symmetric_n-ary_relationship.md#New_comment "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_comment&target=Reviews:AlessandroAdamou_about_Symmetric_n-ary_relationship#New_comment")


Retrieved from "[http://ontologydesignpatterns.org/wiki/Reviews:AlessandroAdamou\_about\_Symmetric\_n-ary\_relationship](../Reviews/AlessandroAdamou_about_Symmetric_n-ary_relationship.md)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [QCReview](../Category/QCReview.md "Category:QCReview")