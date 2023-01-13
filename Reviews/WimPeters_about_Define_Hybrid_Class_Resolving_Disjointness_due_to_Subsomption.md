[![](../images/thumb/2/29/Reviewer.png/48px-Reviewer.png)](../Image/Reviewer.png "Reviewer.png")
__[WimPeters](../User/WimPeters "User:WimPeters") about [Define Hybrid Class Resolving Disjointness due to Subsomption](../Submissions/Define_Hybrid_Class_Resolving_Disjointness_due_to_Subsomption "Submissions:Define Hybrid Class Resolving Disjointness due to Subsomption") (Revision ID: [Hybrid Class Resolving Disjointness due to Subsomption?oldid=5753 5753](../Submissions/Define "http://ontologydesignpatterns.org/wiki/Submissions:Define"))__
Overall suggestion (score): 1 - needs minor revision




 __Review Summary:__ This pattern proposal deserves discussion, in combination with the pattern proposal "Enlarge Class Definition for Resolving Disjointness due to Subsomption", which is a solution variant to the same problem proposed by the same authors.
__Reviewer Confidence:__ medium, having mainly worked with lightweight ontologies.
__Problems:__ Once a subclass is to be defined as a subclass of two disjoint superclasses, this pattern offers a work-around after a more fundamental question has been answered with "yes": Are the two superclasses still to be considered as disjoint?
This is a non-trivial decision, which is borne out by lower than expected levels of agreement between experts (see [http://www.eswc2007.org/pdf/eswc07-voelker1.pdf](http://www.eswc2007.org/pdf/eswc07-voelker1.pdf "http://www.eswc2007.org/pdf/eswc07-voelker1.pdf")).
In description logics two classes are considered as disjoint iff their taxonomic overlap, i.e. the set of common individuals, must be empty in all possible worlds.
As soon as there exists an instance in the extensions of two disjoint superclasses, the engieer is confronted with the following choices:
1. the disjointness axiom should be deleted, which will negatively affect consistency checking and the automatic evaluation of individuals in a knowledge base with regards to a given ontology (again see ([http://www.eswc2007.org/pdf/eswc07-voelker1.pdf](http://www.eswc2007.org/pdf/eswc07-voelker1.pdf "http://www.eswc2007.org/pdf/eswc07-voelker1.pdf")))


2. the proposed pattern should be used. This pattern allows to maintain the original disjoint superclasses while indirectly allowing an instance to be in the extension of both. This goes against the principle of disjointness, but may be convenient in the case where the ontology is imported from another URI.


The pattern defines a hybrid class as a union of the definitions of the disjoint classes. The proposers should indicate more precisely what these definitions consist of. Do they consist of all properties and restrictions?
Is this equivalent to creating a class AnimalOrPlant, or AnimalAndPlant? Is there a difference between the two?



Maybe a third option to be taken into account in the discussion is the introduction of degrees of disjointness.
__Community Relevance:__ high, especially if this pattern is judged as best practise. This type of
__Relation to Best Practices:__ I am not aware of best practise for the solution of this problem.
__Reusability:__ very reusable
__Relations to Other Patterns:__ related pattern proposal:
"Enlarge Class Definition for Resolving Disjointness due to Subsomption"
__Overall Understandability:__ good
__Clear Problem Description:__ 
__Clear Relevance and Consequences:__ It is not clear to me what the union of concept definitions entails.
__Clear Figures and Illustrations:__ Figure is clear. It does not illustrate any relations between DisjointClass 1 and DisjointClass2 on the one hand, and HypbridClass on the other, although the latter is a union of the definitions of the former.
__Missing Information:__ There is no owl version of the pattern. Also, there is no scenario description.

_Posted:_ 2009/9/9 _Last modified:_ 2009/9/9



[All reviews](../Reviews/Main "Reviews:Main") | [Add a comment at the bottom of this page](index.php@title=Odp%253AAdd_comment&target=../Reviews/WimPeters_about_Define_Hybrid_Class_Resolving_Disjointness_due_to_Subsomption#New_comment "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_comment&target=Reviews:WimPeters_about_Define_Hybrid_Class_Resolving_Disjointness_due_to_Subsomption#New_comment")


Retrieved from "[http://ontologydesignpatterns.org/wiki/Reviews:WimPeters\_about\_Define\_Hybrid\_Class\_Resolving\_Disjointness\_due\_to\_Subsomption](../Reviews/WimPeters_about_Define_Hybrid_Class_Resolving_Disjointness_due_to_Subsomption)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [QCReview](../Category/QCReview "Category:QCReview")