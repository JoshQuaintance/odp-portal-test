[![](../images/thumb/2/29/Reviewer.png/48px-Reviewer.png)](../Image/Reviewer.png "Reviewer.png")
__[CatherineRoussey](../User/CatherineRoussey "User:CatherineRoussey") about [SimpleOrAggregated](../Submissions/SimpleOrAggregated "Submissions:SimpleOrAggregated") (Revision ID: [10064](../Submissions/SimpleOrAggregated@oldid=10064 "http://ontologydesignpatterns.org/wiki/Submissions:SimpleOrAggregated?oldid=10064"))__
Overall suggestion (score): 0 - needs major revision




 __Review Summary:__ I do not understand exactly what will be the purpose of this pattern and Which behavior the author expect from the reasoner. So I need more information to give a review. 
The main problem is the semantic of the aggregation property. There exist different partOf relationship and I need to know the relationship between the aggregation property and the partOf one...
__Reviewer Confidence:__ I know the design pattern composite in software engineering...and the DUL ontology. The hasPart and isPartOf property has to be associated to this pattern.
__Problems:__ No information is given on the meaning of the aggregation property: 
is it a hasMember, hasPart, hasComponent property?
maybe the aggregation can be replace by any of them...
and does this property transitive or not?


Why do you thing that all the objects can be classified as a simple one or an aggregated one?
First I would rather fixe a subClassOf relationship between ObjectByCardinality and Object... Depend of the point of view (the scale) an object can be classified as simple or not...
An organ is a simple object or not? Organ is composed of cells and cell is composed of...



if an individual O has two aggregated Members O1 and O2 asserted in the ontology... Moreover if O1 is fixed as same as O2... what do you expect from the reasoner? What's happen if instead 02 is also an aggregatedMember of O1?
__Community Relevance:__ 
__Relation to Best Practices:__ 
__Reusability:__ 
__Relations to Other Patterns:__ 
__Overall Understandability:__ 
__Clear Problem Description:__ This pattern is only applicable in certains conditions which are not well described ...
__Clear Relevance and Consequences:__ The consequence on individual are not well described.
If a whole is composed of two aggregatedMembers which are fixed as equivalent, the whole is still classified as a aggregatedObject.
Is it what do you expect from the reasoner?


Moreover if the whole is classified as a simple Object and is composed of two objects that are equivalent to each other there are an unconsistency...



So I do no think that the reasoning about number of parts is possible with this pattern...
__Clear Figures and Illustrations:__ 
__Missing Information:__ the semantic of the aggregation property: hasAggregatedMember...

_Posted:_ 2010/9/10 _Last modified:_ 2010/9/16



[All reviews](../Reviews/Main "Reviews:Main") | [Add a comment at the bottom of this page](index.php@title=Odp%253AAdd_comment&target=../Reviews/CatherineRoussey_about_SimpleOrAggregated#New_comment "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_comment&target=Reviews:CatherineRoussey_about_SimpleOrAggregated#New_comment")
#####  16-09-2010 [CatherineRoussey](../User/CatherineRoussey "User:CatherineRoussey") says:


I have seen that the definition of a simple Object is an object with no aggregated Objects (no parts) so what is an object with only one aggregated Object? no an aggregated Object but not a simple Object... the ObjectBy Cardinality partition should be modified...





Retrieved from "[http://ontologydesignpatterns.org/wiki/Reviews:CatherineRoussey\_about\_SimpleOrAggregated](../Reviews/CatherineRoussey_about_SimpleOrAggregated)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [QCReview](../Category/QCReview "Category:QCReview")