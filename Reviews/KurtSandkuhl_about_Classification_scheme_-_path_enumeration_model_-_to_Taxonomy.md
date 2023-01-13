[![](../images/thumb/2/29/Reviewer.png/48px-Reviewer.png)](../Image/Reviewer.png "Reviewer.png")
__[KurtSandkuhl](http://ontologydesignpatterns.org/wiki/index.php?title=User:KurtSandkuhl&action=edit&redlink=1 "User:KurtSandkuhl (not yet written)") about [Classification scheme - path enumeration model - to Taxonomy](../Submissions/Classification_scheme_-_path_enumeration_model_-_to_Taxonomy "Submissions:Classification scheme - path enumeration model - to Taxonomy") (Revision ID: [scheme - path enumeration model - to Taxonomy?oldid=5712 5712](../Submissions/Classification "http://ontologydesignpatterns.org/wiki/Submissions:Classification"))__
Overall suggestion (score): 1 - needs minor revision




 __Review Summary:__ Path enumeration is a technique which is quite common in classification schemes. To support re-engineering of such schemes contributes to making them available for semantic applications, which makes the proposed ODP both very relevant and useful.
The basic idea of the pattern and the proposed process are good and require only minor improvements (see detailed comments). But the preconditions for using the pattern and its limitations should be expressed more clearly. Not all existing implementations of the path enumeration scheme are as clean as the UN standards. Path enumeration is not only used with the subClassOf semantics, but also for instanceOf relations. This is mentioned in the description, but should be made more explicit:
Please describe, which preconditions apply for using this pattern (for example: mutually exclusive concept groups, path constitutes unique identifier for concept groups, subClassOf relationship).
An option in this context would be to extend the proposed pattern for cases, when some of the current preconditions do not apply (e.g. other relationships than subClassOf).


Detailed comments:
- the first step in the process description should be re-phrased (unclear wording; what does key value mean in this context?)
- in the graphical representation: the start of a loop is represented in 2 different ways. Please check.
- in “process example” (Example section) you should use the same numbering of the process steps as in the process description. Furthermore, you should also include the first step “identify the classification scheme items” in the example 



The pattern is suitable for presentation at WOP, but might not stimulate a long discussion as the proposed solution – in my opinion is not controversial.
__Reviewer Confidence:__ high
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

_Posted:_ 2009/9/8 _Last modified:_ 2009/9/8



[All reviews](../Reviews/Main "Reviews:Main") | [Add a comment at the bottom of this page](index.php@title=Odp%253AAdd_comment&target=../Reviews/KurtSandkuhl_about_Classification_scheme_-_path_enumeration_model_-_to_Taxonomy#New_comment "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_comment&target=Reviews:KurtSandkuhl_about_Classification_scheme_-_path_enumeration_model_-_to_Taxonomy#New_comment")


Retrieved from "[http://ontologydesignpatterns.org/wiki/Reviews:KurtSandkuhl\_about\_Classification\_scheme\_-\_path\_enumeration\_model\_-\_to\_Taxonomy](../Reviews/KurtSandkuhl_about_Classification_scheme_-_path_enumeration_model_-_to_Taxonomy)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [QCReview](../Category/QCReview "Category:QCReview")