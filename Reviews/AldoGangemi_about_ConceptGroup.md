[![](../images/thumb/2/29/Reviewer.png/48px-Reviewer.png)](../Image/Reviewer.png.md "Reviewer.png")
__[AldoGangemi](../User/AldoGangemi.md "User:AldoGangemi") about [ConceptGroup](../Submissions/ConceptGroup.md "Submissions:ConceptGroup") (Revision ID: [5807](../Submissions/ConceptGroup@oldid=5807.md "http://ontologydesignpatterns.org/wiki/Submissions:ConceptGroup?oldid=5807"))__
Overall suggestion (score): 0 - needs major revision




 __Review Summary:__ The pattern tries to provide an OWL representation of a construct used to talk about groups of concepts or fragments of thesauri.
I think the pattern is a valid contribution, but needs major revisions in documentation, axiomatization, and relation to other patterns.
__Reviewer Confidence:__ High
__Problems:__ The lack of a concrete example makes the pattern difficult to understand. From the technical viewpoint, there are some problems:
1) the object properties lack inverses: this is a bad practice; inGroup lacks an inverse at all, while BT is not made inverse of NT, and subGroup of superGroup
2) the reification of BT-NT, and subGroup-superGroup mught be due to the need of creating inverse object properties: in this case, this is a bad practice. If reifications are needed for other reasons, this is not clear



3) the structuringAssociationType object property seems used to link concept groups to the reification of BT-NT. Why is is needed? The use case behind this object property is unclear
__Community Relevance:__ Fair
__Relation to Best Practices:__ The pattern allows to represent groups of concepts, in that being a special case of the CollectionEntity pattern (Collection <- Group, Thing <- Concept, memberOf <- inGroup).
Moreover, it seems to encode also:
a) a subgroup relation (could be kind of partof for collections)
b) the BT relation (already existing in SKOS core, but could also be kind of specialization for concepts, see also Specialization and Classification patterns)
c) a "membership restriction" class that is basically synonym to Group



I think this pattern can be represented in a simplier way (see Problems above)
__Reusability:__ Good, if the problems are solved
__Relations to Other Patterns:__ CollectionEntity can be specialized for the core part of this pattern.
Classification and Specialization are also related.



SKOS (potentially a content pattern has also overlaps).
__Overall Understandability:__ Low
__Clear Problem Description:__ Must be explained better
__Clear Relevance and Consequences:__ Must be explained better
__Clear Figures and Illustrations:__ Ok
__Missing Information:__ Concrete example. I also suggest to load the annotations in the OWL file, not just on the portal.

_Posted:_ 2009/9/12 _Last modified:_ 2009/9/12



[All reviews](../Reviews/Main.md "Reviews:Main") | [Add a comment at the bottom of this page](index.php@title=Odp%253AAdd_comment&target=../Reviews/AldoGangemi_about_ConceptGroup.md#New_comment "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_comment&target=Reviews:AldoGangemi_about_ConceptGroup#New_comment")


Retrieved from "[http://ontologydesignpatterns.org/wiki/Reviews:AldoGangemi\_about\_ConceptGroup](../Reviews/AldoGangemi_about_ConceptGroup.md)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [QCReview](../Category/QCReview.md "Category:QCReview")