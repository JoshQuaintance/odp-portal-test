[![](../images/thumb/2/29/Reviewer.png/48px-Reviewer.png)](../Image/Reviewer.png.md "Reviewer.png")
__[RimDJEDIDI](../User/RimDJEDIDI.md "User:RimDJEDIDI") about [Classification scheme - adjacency list model - to Taxonomy](../Submissions/Classification_scheme_-_adjacency_list_model_-_to_Taxonomy.md "Submissions:Classification scheme - adjacency list model - to Taxonomy") (Revision ID: [scheme - adjacency list model - to Taxonomy?oldid=5625 5625](../Submissions/Classification.md "http://ontologydesignpatterns.org/wiki/Submissions:Classification"))__
Overall suggestion (score): 1 - needs minor revision




 __Review Summary:__ This re-engineering pattern is proposed for re-engineering a non-ontological resource following the adjacency list model to design a taxonomy. 
Suitability for WOP discussion: Relevant



Pattern Quality: an interesting initial version to be enriched
__Reviewer Confidence:__ ODPs in general : High
The addressed Problem (adjacency list model): Medium



Taxonomy modeling : High
__Problems:__ 1- The non-ontological resource (adjacency list model) re-engineered by this pattern is described as a rooted tree of concepts grouped by some particular degree of similarity. But it is stated that the semantics of hierarchical relation between concepts may vary depending on the context. So, if the relation between adjacency list entities related by a linking column (and expressed by the column title) is more rich than a kind of similarity or a generalization, re-engineering it to a taxonomy classification (mapping the relationship to a subClassOf relation) may reduce the original semantic relation between concepts.
2- There is no reference to the multi-inheritance case, however it is implicitly supported by the process. It should be explicitly clarified whether it is considered in this re-engineering or not modeled in a adjacency list.



3- Cyclic relationship: as a consequence to the first problem described above, a mutual relation between adjacency list concepts may lead to cyclic relation in the taxonomy when applying the process. The hierarchical structure of a taxonomy is typically organized by a subClassOf relation. So, cyclic relation will lead to confusing modeling of subClassOf, equivalent and symmetric semantic relations.
__Community Relevance:__ the intent of the pattern targets a relevant problem in re-engineering non-ontological resources which is how to re-engineer an adjacency list model? However, it needs to include more related issues.
__Relation to Best Practices:__ 
__Reusability:__ The pattern could be unsuitable for some kind of adjacency list. Its usability should be explicitly defined to avoid inappropriate reuse.
__Relations to Other Patterns:__ 
__Overall Understandability:__ The pattern description is understandable. May be for documentation purpose and to facilitate its reuse particularly for novice or learner users, it would be more clear to add a definition for the different parameters used in the process at the beginning of its description.
__Clear Problem Description:__ In the "non-ontological resource description" property, it is stated that the considered classification is a rooted tree, so if this means that adjacency list cannot represent a graph, it should be mentioned explicitly to avoid ambiguity about cyclic relation. 
Besides, it should be made precise whether the re-engineering is specifically proposed to hierarchical classification adjacency list.



In summary, it should be specified under what conditions the pattern is applicable. A proposition could be to add a property "Applicability" to pattern description template?
__Clear Relevance and Consequences:__ 
__Clear Figures and Illustrations:__ Figures are clear however, the diagram illustrating the re-engineering process are incomplete and should include the recursive mechanism (2.3.3 step) and the final step of creating the hierarchy's root.
__Missing Information:__ 

_Posted:_ 2009/9/7 _Last modified:_ 2009/9/7



[All reviews](../Reviews/Main.md "Reviews:Main") | [Add a comment at the bottom of this page](index.php@title=Odp%253AAdd_comment&target=../Reviews/RimDJEDIDI_about_Classification_scheme_-_adjacency_list_model_-_to_Taxonomy.md#New_comment "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_comment&target=Reviews:RimDJEDIDI_about_Classification_scheme_-_adjacency_list_model_-_to_Taxonomy#New_comment")


Retrieved from "[http://ontologydesignpatterns.org/wiki/Reviews:RimDJEDIDI\_about\_Classification\_scheme\_-\_adjacency\_list\_model\_-\_to\_Taxonomy](../Reviews/RimDJEDIDI_about_Classification_scheme_-_adjacency_list_model_-_to_Taxonomy.md)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [QCReview](../Category/QCReview.md "Category:QCReview")