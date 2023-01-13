[![](../images/thumb/2/29/Reviewer.png/48px-Reviewer.png)](../Image/Reviewer.png "Reviewer.png")
__[AlessandroAdamou](../User/AlessandroAdamou "User:AlessandroAdamou") about [Reactor pattern](../Submissions/Reactor_pattern "Submissions:Reactor pattern") (Revision ID: [pattern?oldid=11155 11155](../Submissions/Reactor "http://ontologydesignpatterns.org/wiki/Submissions:Reactor"))__
Overall suggestion (score): 1 - needs minor revision




 __Review Summary:__ The pattern brings a nontrivial modeling problem to the domain of process and workflow representation. 
If the pattern is revised to reuse existing patterns, provides less in-house namespacing and integrates more entity annotations, it will be a fine addition and a prime candidate for the catalogue. To that end, it would be good to issue a revised version with its own version IRI.



Some rather feasible presentation issues in the pattern page should be addressed as well.
__Reviewer Confidence:__ High (ontologies, OWL, ontology design patterns), Medium (process modeling)
__Problems:__ - From the competency questions, it is not clear if input, output, conditions and triggers (events) need to be instantiated as actual values, or simply \*categories\* of parameters, conditions and events.
- Wouldn't it be possible to relax existential restrictions on input/output parameters for the Process class?



- Typo: Property "hasEnvironemntalCondition" should be "hasEnvironmentalCondition"
__Community Relevance:__ High, due to its attempt at tackling the cause/effect representation problem and bringing it to the domain of process models.
__Relation to Best Practices:__ It could set a standard solution for process modeling in various domains, provided that its relation with patterns like Parameter and Reaction is well-defined.
__Reusability:__ Reusable, with the possible drawback of namespacing. Every entity is defined in-house with namespace "[http://purl.org/biomass/ReactorPattern#](http://purl.org/biomass/ReactorPattern# "http://purl.org/biomass/ReactorPattern#")", which means that if I reuse this pattern, it could remain isolated from other imported definitions of Process, Event, etc. unless I manually align them. The pattern itself should reuse these base concepts.
__Relations to Other Patterns:__ It would probably be better off specializing some other content pattern, e.g. Reaction.
The "Parameter" pattern could also be specialized.
__Overall Understandability:__ The intent and implementation are very clear, sans the issues described in other fields.
__Clear Problem Description:__ Clear, but it seems to tackle two problems, i.e. parametric processes and cause/effect relations. Content Patterns should be atomic solutions whenever possible.
__Clear Relevance and Consequences:__ Clear. Thers's one extra newline in the "Consequences" field.
__Clear Figures and Illustrations:__ Clear and understandable, though it would be better to develop the figure vertically a little more.
__Missing Information:__ - Labels and comments for most entities
- There is a scenario annotation in the ontology - It would be good to add a more elaborate version of it to the "Scenarios" section of the pattern page (not just the field in the general description).
- The OntoMDL implementation should be mentioned (with a link to the ontology) in the "Known Uses" field.



- I personally would suggest that Content Patterns start to use OWL 2 version IRI, given that they are subject to refinement -> versioning. Please note that version IRIs should resolve to the specific version of the ontology, while the ontology IRI should resolve to the latest stable release.

_Posted:_ 2012/8/24 _Last modified:_ 2012/8/24



[All reviews](../Reviews/Main "Reviews:Main") | [Add a comment at the bottom of this page](index.php@title=Odp%253AAdd_comment&target=../Reviews/AlessandroAdamou_about_Reactor_pattern#New_comment "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_comment&target=Reviews:AlessandroAdamou_about_Reactor_pattern#New_comment")


Retrieved from "[http://ontologydesignpatterns.org/wiki/Reviews:AlessandroAdamou\_about\_Reactor\_pattern](../Reviews/AlessandroAdamou_about_Reactor_pattern)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [QCReview](../Category/QCReview "Category:QCReview")