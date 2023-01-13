[![](../../images/thumb/2/29/Reviewer.png/48px-Reviewer.png)](../../Image/Reviewer.png "Reviewer.png")
__[EnricoDaga](../../User/EnricoDaga "User:EnricoDaga") about [Xsd:sequence embedding](../../Submissions/Xsd/sequence_embedding "Submissions:Xsd:sequence embedding") (Revision ID: [embedding?oldid=5723 5723](../../Submissions/Xsd/sequence "http://ontologydesignpatterns.org/wiki/Submissions:Xsd:sequence"))__
Overall suggestion (score): 0 - needs major revision




 __Review Summary:__ This submission needs major revision. It is not clear if the aim is to model a partitive relation between embedded xml elements to the relative parent element in general or in particular for the xsd:sequence element. In the second case the partOf property defined in DOLCE is not enough, better use the [Submission:Sequence](http://ontologydesignpatterns.org/wiki/index.php?title=Submission:Sequence&action=edit&redlink=1 "Submission:Sequence (not yet written)") pattern. In the first case the pattern should be focused on the xsd:all element instead. Additionally, a reengineering pattern for partitive relation in XML-based documents is more general then the XSD case, and probably should be approached at that level, focusing on XSD case in the example section.
__Reviewer Confidence:__ The submission should be revised for the meaning described above. Anyway the problem of reengineering XML-based structures to patterns should be faced in the near future by the community. Revised properly, this proposal could be a good starting point.
__Problems:__ This pattern is named XSD:Sequence embedding. The 'sequence' indicator in XSD means not only a group of element into another (as xsd:all or rdf:Bag), but implies also the fact that those elements must be in a particular order, and this order cannot change, or if it changes, or it is lost in the reengeneering process, the result is a loss of information (see, for example [[1]](http://www.w3schools.com/schema/schema_complex_indicators.asp "http://www.w3schools.com/schema/schema_complex_indicators.asp")).
The semantic of the 'partOf' ObjectProperty defines pure meronimy relation. It is probably the good solution for representing the containment of one or more XML elements into another (also rdf:Bag could be reengineered in an ontology in the same way). In the XSD case, it can be used to reengineer the 'All' order indicator instead of the 'sequence' one.


Additionally, the example refers to the case in wich the order of the embedded elements is not important. 


There are two possibilities:
1) The pattern should be renamed, removing the relation to the 'sequence' and changing it into 'meronimy' or 'partitive' relation, taking the example as meaningful



2) The sequence is a crucial point of this pattern, and this should be better motivated in the example and description of the process.
__Community Relevance:__ The problem of reengineering XML-based structures to patterns should be faced in the near future by the community. A revised version of this pattern could have a place in that scenario.
__Relation to Best Practices:__ Actually no relation to best practices. Also this point should be take into account in future revisions of this submissions.
__Reusability:__ Not evaluable at the moment.
__Relations to Other Patterns:__ [Submissions:PartOf](../../Submissions/PartOf "Submissions:PartOf"), [Submissions:Sequence](../../Submissions/Sequence "Submissions:Sequence")
__Overall Understandability:__ Actually the aim is not clear.
__Clear Problem Description:__ As above.
__Clear Relevance and Consequences:__ Not clear at the moment.
__Clear Figures and Illustrations:__ Not evaluable at the moment.
__Missing Information:__ A clear report about the usage and meaning of the xs:sequence element in XSD could be added.

_Posted:_ 2009/9/8 _Last modified:_ 2009/9/8



[All reviews](../../Reviews/Main "Reviews:Main") | [Add a comment at the bottom of this page](index.php@title=Odp%253AAdd_comment&target=../../Reviews/EnricoDaga_about_Xsd/sequence_embedding#New_comment "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_comment&target=Reviews:EnricoDaga_about_Xsd:sequence_embedding#New_comment")


Retrieved from "[http://ontologydesignpatterns.org/wiki/Reviews:EnricoDaga\_about\_Xsd:sequence\_embedding](../../Reviews/EnricoDaga_about_Xsd/sequence_embedding)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [QCReview](../../Category/QCReview "Category:QCReview")