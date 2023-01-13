[![](../images/thumb/2/29/Reviewer.png/48px-Reviewer.png)](../Image/Reviewer.png "Reviewer.png")
__[StefanoDavid](../User/StefanoDavid "User:StefanoDavid") about [OnlynessIsLoneliness (OIL)](../Submissions/OnlynessIsLoneliness_(OIL)).md).md).html "Submissions:OnlynessIsLoneliness (OIL)") (Revision ID: [(OIL)?oldid=5787 5787](../Submissions/OnlynessIsLoneliness "http://ontologydesignpatterns.org/wiki/Submissions:OnlynessIsLoneliness"))__
Overall suggestion (score): 1 - needs minor revision




 __Review Summary:__ The authors propose a solution to a common modeling error, the use of disjointness assertions, that causes inconsistencies.
__Reviewer Confidence:__ Good knowledge in Description logics and OWL
__Problems:__ \* I would rephrase the problem statement: I would suggest to call "problem" the modeling error (which is obviously an Anti-Pattern, as it causes the ontology to become useless), and "pattern" the proposed solution.
* There are different hydrontologies in the "Pattern solution example": I would point only to one of them, as they seem very similar, and use it also as use case.


* Although the hydrontologies seem to be some official Spanish knowledge bases, I would rather use an english version of a part of them that clearly states the problem, as it is not so comfortable to search in the whole ontology the pattern.


* I would extend the definition of this pattern by suggesting that it is allowed the use of multiple restrictions (i.e., C1 subClassOf R only C2, ... ,C1 subClassOf R only Cn) to be combined in a single disjointness axiom, e.g., for those languages, like OWL2, that allow DisjointClasses into a single axiom:


C1 subClassOf R only (C2 or ... or Cn); disjointClasses (C2, ... Cn)



* "We have categorized them into three groups:". There are no three groups in the remainder, but the description of three classes


__Community Relevance:__ Medium/High, since the wrong use and the misuse of disjointness is often difficult to spot.
__Relation to Best Practices:__ High, as it solves modeling mistakes.
__Reusability:__ Yes, across different languages and every time a (wrongly defined) disjointness is involved
__Relations to Other Patterns:__ 
__Overall Understandability:__ The modeling problem and proposed solutions need a rewording, but the purpose is clear.
__Clear Problem Description:__ No, it needs some rework.
__Clear Relevance and Consequences:__ yes
__Clear Figures and Illustrations:__ None provided
__Missing Information:__ ER/UML diagram

_Posted:_ 2009/9/10 _Last modified:_ 2009/9/10



[All reviews](../Reviews/Main "Reviews:Main") | [Add a comment at the bottom of this page](index.php@title=Odp%253AAdd_comment&target=../Reviews/StefanoDavid_about_OnlynessIsLoneliness_(OIL)).md).md).html#New_comment "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_comment&target=Reviews:StefanoDavid_about_OnlynessIsLoneliness_(OIL)#New_comment")


Retrieved from "[http://ontologydesignpatterns.org/wiki/Reviews:StefanoDavid\_about\_OnlynessIsLoneliness\_%28OIL%29](../Reviews/StefanoDavid_about_OnlynessIsLoneliness_(OIL)).md).md).html)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [QCReview](../Category/QCReview "Category:QCReview")