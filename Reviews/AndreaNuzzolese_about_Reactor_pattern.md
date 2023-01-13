[![](../images/thumb/2/29/Reviewer.png/48px-Reviewer.png)](../Image/Reviewer.png "Reviewer.png")
__[AndreaNuzzolese](../User/AndreaNuzzolese "User:AndreaNuzzolese") about [Reactor pattern](../Submissions/Reactor_pattern "Submissions:Reactor pattern") (Revision ID: [pattern?oldid=11175 11175](../Submissions/Reactor "http://ontologydesignpatterns.org/wiki/Submissions:Reactor"))__
Overall suggestion (score): 1 - needs minor revision




 __Review Summary:__ The pattern addresses a relavant problem in modeling reactive processes. The problem statement and the solution presented and proposed by the author are clear. The terminology used for naming classes and properties is appropriate with respect to the context. Competency questions proposed are exhaustive for expressing the requirements that should be covered by the patterns.
In my opinion there is a lack of usage of existing content pattern. For example the ProcessParameter class can be defined by specializing the Parameter class from the parameter pattern ([http://ontologydesignpatterns.org/cp/owl/parameter.owl](http://ontologydesignpatterns.org/cp/owl/parameter.owl "http://ontologydesignpatterns.org/cp/owl/parameter.owl")). 
I also see an Event as a n-ary relation. This allows to express the Event class by specializing the Situation content pattern.


I don't understand the need of the definition of the description object property. If its intent is to express the descriptive context of a concept the Description pattern could be used. Otherwise an annotation property or even the rdfs:comment could be used.


I find the existential restriction for the Process class to strict for what is used as a top level class.



The author is encouraged to use labels and comments for entities defined in the pattern.
__Reviewer Confidence:__ High
__Problems:__ There is a typo in the hasEnvironemntalCondition object property that should be hasEnvironmentalCondition.
Labels and comments should be defined for each class and property in the pattern.
__Community Relevance:__ The relevance is high.
__Relation to Best Practices:__ As described in the summary existing content patterns should be used by the Reactor pattern.
__Reusability:__ The design adopted makes the pattern highly. The only remark is the existential restriction for the Process class, which in my opinion is to strict for a top level class in a pattern for representing general reactive processes.
__Relations to Other Patterns:__ A similar pattern in the ODP repository is the reaction pattern.
__Overall Understandability:__ 
__Clear Problem Description:__ 
__Clear Relevance and Consequences:__ 
__Clear Figures and Illustrations:__ 
__Missing Information:__ 

_Posted:_ 2012/8/29 _Last modified:_ 2012/8/29



[All reviews](../Reviews/Main "Reviews:Main") | [Add a comment at the bottom of this page](index.php@title=Odp%253AAdd_comment&target=../Reviews/AndreaNuzzolese_about_Reactor_pattern#New_comment "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_comment&target=Reviews:AndreaNuzzolese_about_Reactor_pattern#New_comment")


Retrieved from "[http://ontologydesignpatterns.org/wiki/Reviews:AndreaNuzzolese\_about\_Reactor\_pattern](../Reviews/AndreaNuzzolese_about_Reactor_pattern)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [QCReview](../Category/QCReview "Category:QCReview")