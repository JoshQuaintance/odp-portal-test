[![](../images/thumb/2/29/Reviewer.png/48px-Reviewer.png)](../Image/Reviewer.png "Reviewer.png")
__[VojtechSvatek](../User/VojtechSvatek "User:VojtechSvatek") about [Classification scheme - adjacency list model - to Taxonomy](../Submissions/Classification_scheme_-_adjacency_list_model_-_to_Taxonomy "Submissions:Classification scheme - adjacency list model - to Taxonomy") (Revision ID: [scheme - adjacency list model - to Taxonomy?oldid=5681 5681](../Submissions/Classification "http://ontologydesignpatterns.org/wiki/Submissions:Classification"))__
Overall suggestion (score): 0 - needs major revision




 __Review Summary:__ A reengineering pattern for a predefined type of tabular structure. Semantic aspects are not taken into account. There are some inconsistencies in the description. 
However, it is a good starting point for discussion at WOP. I assume it should be explained in the context of reengineering patterns in general.
__Reviewer Confidence:__ The problem is relatively transparent and the domain is generic, so I have high confidence in my assessment.
__Problems:__ 1) Although the semantics of the hierarchical relation 'may vary depending of the context', there are no alternative modelling options offered; the subclass construct is uniformly used, which has the subset semantics; this may lead to discrepancies if the original resource is e.g. partonomy-oriented. This should at least be commented on, as a limitation of the pattern usage.
2) While the problem description assumes that the original source is structured as tree, the process description has a special provision for non-tree structures. This is confusing.


3) When a new 'ad hoc' class is created, it is not clear if it is to be identified with a standard class such as owl:Thing, or given the URI through some naming convention - I would expect such a convention as natural part of the pattern.


Text-level issues:
- what is caparentID?



- the last diagram (at example level) is trivial and could safely be omitted
__Community Relevance:__ This kind of patterns is naturally important, as reengineering of non-ontological resources is an ubiquitous problem.
__Relation to Best Practices:__ The problem is simplified such that the current pattern looks like the only straightforward solution. In reality a more complex solution would be needed.
__Reusability:__ The pattern is specific to a particular category of non-ontological resources. However, its abstract part could be reused for some other categories.
__Relations to Other Patterns:__ Obviously, the same non-ontological resources could be transformed to a different ontological form (such as instance-level), presumably using an alternative reengineering pattern.
__Overall Understandability:__ Understandable, even a bit too verbose in places.
__Clear Problem Description:__ As mentioned, the problem is oversimplified. The description of the simple problem, i.e. mechanically transforming a table into an ontology, is clear.
__Clear Relevance and Consequences:__ Not much.
__Clear Figures and Illustrations:__ Clear, and a bit trivial.
__Missing Information:__ 

_Posted:_ 2009/9/8 _Last modified:_ 2009/9/8



[All reviews](../Reviews/Main "Reviews:Main") | [Add a comment at the bottom of this page](index.php@title=Odp%253AAdd_comment&target=../Reviews/VojtechSvatek_about_Classification_scheme_-_adjacency_list_model_-_to_Taxonomy#New_comment "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_comment&target=Reviews:VojtechSvatek_about_Classification_scheme_-_adjacency_list_model_-_to_Taxonomy#New_comment")


Retrieved from "[http://ontologydesignpatterns.org/wiki/Reviews:VojtechSvatek\_about\_Classification\_scheme\_-\_adjacency\_list\_model\_-\_to\_Taxonomy](../Reviews/VojtechSvatek_about_Classification_scheme_-_adjacency_list_model_-_to_Taxonomy)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [QCReview](../Category/QCReview "Category:QCReview")