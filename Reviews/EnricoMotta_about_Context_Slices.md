[![](../images/thumb/2/29/Reviewer.png/48px-Reviewer.png)](../Image/Reviewer.png.md "Reviewer.png")
__[EnricoMotta](../User/EnricoMotta.md "User:EnricoMotta") about [Context Slices](../Submissions/Context_Slices.md "Submissions:Context Slices") (Revision ID: [Slices?oldid=10119 10119](../Submissions/Context.md "http://ontologydesignpatterns.org/wiki/Submissions:Context"))__
Overall suggestion (score): 1 - needs minor revision




 __Review Summary:__ This is a very interesting and useful pattern providing a generic solution to a modelling problem which is more or less ubiquitous when using KR techniques to solve real world problems. However, the description of the pattern (in particular, motivation and pros and cons of the solution) is a bit unclear in parts and ought to be improved, esp. to clarify the pros and cons of the solution to users who may have enough knowledge to apply the pattern to a modelling problem but are not necessarily familiar with all the finer points of meta-level KR.
__Reviewer Confidence:__ High
__Problems:__ There are no errors in the conceptual description of the pattern, however the OWL version of the pattern does not load properly in either topbraid or neon. As an additional minor point, I suspect the arrow ceoOf in the graphical representation is going the wrong way.
__Community Relevance:__ This is a very interesting and useful pattern providing a generic solution to a modelling problem which is more or less ubiquitous when using KR techniques to solve real world problems.
__Relation to Best Practices:__ There are several ways to address this problem in the literature, the most obvious one involving the use of reification to be able to make statements about a triple, such as its contextual extent. The author claims that his solution has advantages over reification-based alternative solutions, however the argument is not entirely clear and some clarifications will make it easier for users to understand better the advantages of this solution - see below for more details on this point.
__Reusability:__ The pattern is very generic and reusable in several situations where context modelling is needed.
__Relations to Other Patterns:__ 
__Overall Understandability:__ The description of the pattern says:
“In RDF and other binary relation languages (like object oriented languages and description logics), one typical way to represent that a binary relation holds in some context is to "reify" the relation-holding (sometimes called obtainment) in the context as an object with a binary relation between the obtainment and each the two relation arguments and a third binary relation between the obtainment and an object representing the context itself. The downside to this approach is the expressive ability of the language to describe the binary relation, especially in the case of description logics, is lost.”


Actually, this is not completely clear. The standard way to do reification in RDF is simply to reformulate a triple using the built-in RDF support. This allows then one to make statements about a triple, such as <triple1, holds, context1>. However, reifying a triple is an additional operation to representing the original statement, e.g., <Sam, ceoOf, IBM>, hence it is not clear why the proposed pattern is an improvement in this respect, given that also a reification-based solution permits to model the original domain-level relation – in this case, ceoOf. 


Another thing that hampers understanding is that the term 'obtainment' does not seem to be a standard one in the literature. I could not find any use of it and indeed, even the referenced paper by Welty and Fikes does not use this term!!! Hence, it is difficult for the reader to completely understand the obtainment-based alternative and I suggest that this part is clarified. 


It is also not clear whether having two IBMs and two Sams in the model causes potential problems. Can one say <sam@c1 sameAs sam>? Probably not. But then how do I retrieve all properties of Sam? 



Related to the above point, it is also unclear what is the semantics of projectionOf.
__Clear Problem Description:__ The problem description is reasonably clear. However, because the example used is "Chris believes..." and the "Chris believes" bit is not actually represented, it would be useful to clarify explicitly whether this solution is adequate to model the different beliefs of different people, or whether "Chris believes" is simply considered as an atomic context and more machinery (i.e., more patterns) would be needed if we also want to add an entity called Chris to the model and relate this to his beliefs.
__Clear Relevance and Consequences:__ 
__Clear Figures and Illustrations:__ yes
__Missing Information:__ 

_Posted:_ 2010/9/19 _Last modified:_ 2010/9/19



[All reviews](../Reviews/Main.md "Reviews:Main") | [Add a comment at the bottom of this page](index.php@title=Odp%253AAdd_comment&target=../Reviews/EnricoMotta_about_Context_Slices.md#New_comment "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_comment&target=Reviews:EnricoMotta_about_Context_Slices#New_comment")


Retrieved from "[http://ontologydesignpatterns.org/wiki/Reviews:EnricoMotta\_about\_Context\_Slices](../Reviews/EnricoMotta_about_Context_Slices.md)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [QCReview](../Category/QCReview.md "Category:QCReview")