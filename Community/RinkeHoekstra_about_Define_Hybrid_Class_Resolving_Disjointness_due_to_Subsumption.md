[![](../images/thumb/a/a6/ODPUser.png/48px-ODPUser.png)](../Image/ODPUser.png "ODPUser.png")
__[RinkeHoekstra](../User/RinkeHoekstra "User:RinkeHoekstra") about [Define Hybrid Class Resolving Disjointness due to Subsumption](../Submissions/Define_Hybrid_Class_Resolving_Disjointness_due_to_Subsumption "Submissions:Define Hybrid Class Resolving Disjointness due to Subsumption") (Revision ID: [Hybrid Class Resolving Disjointness due to Subsumption?oldid=5867 5867](../Submissions/Define "http://ontologydesignpatterns.org/wiki/Submissions:Define"))__
Overall suggestion (score): -1 - reject




 __Review Summary:__ The reason I propose to reject this pattern is that it is decidedly silly.
The authors say that "The definition of the Hybrid Class is the union (OR) of the definitions of the disjoint classes." 


The reason is that the two classes A and B are subsumed by their union A V B. What the pattern does is that we leave implicit what the __proper__ type of the individual is: we simply do not know whether the individual is in A or B.
However, any individual instance of A V B will always be either in A or in B, but __never__ in both (since this is what disjointness specifies). 



The example therefore does not applies. If Animal\_Plant is defined as the union of Animal and Plant (both disjoint) then there still exist no Animal\_Plant instances... and this is what the pattern supposedly tries to solve.
__Reviewer Confidence:__ 
__Problems:__ 
__Community Relevance:__ 
__Relation to Best Practices:__ 
__Reusability:__ 
__Relations to Other Patterns:__ 
__Overall Understandability:__ 
__Clear Problem Description:__ 
__Clear Relevance and Consequences:__ 
__Clear Figures and Illustrations:__ 
__Missing Information:__ 

_Posted:_ 2009-10-25 _Last modified:_ 2009/10/25



[All reviews](../Reviews/Main "Reviews:Main") | [Add a comment at the bottom of this page](index.php@title=Odp%253AAdd_comment&target=../Community/RinkeHoekstra_about_Define_Hybrid_Class_Resolving_Disjointness_due_to_Subsumption#New_comment "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_comment&target=Community:RinkeHoekstra_about_Define_Hybrid_Class_Resolving_Disjointness_due_to_Subsumption#New_comment")


Retrieved from "[http://ontologydesignpatterns.org/wiki/Community:RinkeHoekstra\_about\_Define\_Hybrid\_Class\_Resolving\_Disjointness\_due\_to\_Subsumption](../Community/RinkeHoekstra_about_Define_Hybrid_Class_Resolving_Disjointness_due_to_Subsumption)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [OpenReview](../Category/OpenReview "Category:OpenReview")