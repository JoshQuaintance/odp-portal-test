[![](../images/thumb/2/29/Reviewer.png/48px-Reviewer.png)](../Image/Reviewer.png.md "Reviewer.png")
__[MariaPoveda](../User/MariaPoveda.md "User:MariaPoveda") about [OOPMetrics](../Submissions/OOPMetrics.md "Submissions:OOPMetrics") (Revision ID: [11161](../Submissions/OOPMetrics@oldid=11161.md "http://ontologydesignpatterns.org/wiki/Submissions:OOPMetrics?oldid=11161"))__
Overall suggestion (score): 0 - needs major revision




 __Review Summary:__ The patterns describes numerical values (float and integer) for onject-oriented software metrics.
The pattern is reusable and general enough.



There are some revisions needed.
__Reviewer Confidence:__ High
__Problems:__ Main comments:
.- The domain of the relationship "hasMetric" is set as the intersection of serveral classes, namely OOPClass, OOPProject, OOPMethod and OOPPackage. I think it should be defined as the union of theses classes so that if a instance holds this property it is not classified as instance of all these types, that might be disjoint, when running a reasoner over the ontology.


.- The CPAnnotation schema is not imported in the OWL building block as stated in the call. It would be great if the pattern were annotated using such a schema.


.- There are no labels nor comments in the OWL code.


Minor comments:


.- The already existing domain "software" should be added to the domains field.



.- The figure could be improved by including the datatype properties.
__Community Relevance:__ Good
__Relation to Best Practices:__ 
__Reusability:__ Good
__Relations to Other Patterns:__ 
__Overall Understandability:__ Even though the understandability is good, it would be advisable to explain in more detail the solution description.
__Clear Problem Description:__ Good
__Clear Relevance and Consequences:__ Good
__Clear Figures and Illustrations:__ The figure could be improved by including the datatype properties.
__Missing Information:__ 

_Posted:_ 2012/8/21 _Last modified:_ 2012/8/21



[All reviews](../Reviews/Main.md "Reviews:Main") | [Add a comment at the bottom of this page](index.php@title=Odp%253AAdd_comment&target=../Reviews/MariaPoveda_about_OOPMetrics.md#New_comment "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_comment&target=Reviews:MariaPoveda_about_OOPMetrics#New_comment")


Retrieved from "[http://ontologydesignpatterns.org/wiki/Reviews:MariaPoveda\_about\_OOPMetrics](../Reviews/MariaPoveda_about_OOPMetrics.md)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [QCReview](../Category/QCReview.md "Category:QCReview")