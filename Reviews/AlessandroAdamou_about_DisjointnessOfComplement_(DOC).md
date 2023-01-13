[![](../images/thumb/2/29/Reviewer.png/48px-Reviewer.png)](../Image/Reviewer.png "Reviewer.png")
__[AlessandroAdamou](../User/AlessandroAdamou "User:AlessandroAdamou") about [DisjointnessOfComplement (DOC)](../Submissions/DisjointnessOfComplement_(DOC)).md).md).html "Submissions:DisjointnessOfComplement (DOC)") (Revision ID: [(DOC)?oldid=5597 5597](../Submissions/DisjointnessOfComplement "http://ontologydesignpatterns.org/wiki/Submissions:DisjointnessOfComplement"))__
Overall suggestion (score): 1 - needs minor revision




 __Review Summary:__ The proposal looks sensible to me, but I do expect that other peers might believe it to be rather trivial, thus I would recommend it for discussion at WOP. It is however essential that this proposal is presented in such a way as to target naive developers.
__Reviewer Confidence:__ ODPs: medium/high
Description Logics: medium
__Problems:__ Nothing in particular as for the pattern itself. For the presentation, see below.
__Community Relevance:__ This proposal could bring up some fruitful discussion during the workshop. I, for one, had never even thought about the very existence of such a pitfall in ontology engineering, and the first time I read it I was questioning the actual utility of such a pattern, though some more thorough analysis made me change my mind.
__Relation to Best Practices:__ 
__Reusability:__ I'm reasonably sure it is unwittingly being used in many ontology design activities as I write. At least I hope so.
__Relations to Other Patterns:__ 
__Overall Understandability:__ Immediate for the knowledgeable ontology developer, but since the proposal is aimed at solving a trivial yet possibly frequent issue, maybe a step-by-step explanation "for dummies" on how to use it could help. See suggestions below. 
In addition, at least one more ontology providing a solution example in English should be posted.
__Clear Problem Description:__ This aspect should be developed in more detail. Please bear in mind that this description should be thorough enough to aid all ontology engineers, let alone the least experienced ones.
Since we are mentioning logical antipatterns, I think a couple of examples showing the bizarre consequences of a failure to apply such a pattern would help. Like, say, showing how statements such as : 


- SaltLake isEquivalentTo not FreshWaterLake  

- Balkhash isA SaltLake  

- SpiderMan isDifferentFrom Balkhash  




then reasoning could infer that SpiderMan is a FreshWaterLake. Anyway, the more absurd and shocking the examples, the higher the chance for inexperienced ontology developers to get it right.
__Clear Relevance and Consequences:__ As per problem description, the authors should display how such bizarre phenomena should not occur if disjointness is used instead.
__Clear Figures and Illustrations:__ I obviously do not expect a "classic ontology" diagram, but an illustration depicting the difference between the two types of statements is strongly recommended. A couple of Venn diagrams, one for complement and one for disjointness, should do fine.
__Missing Information:__ Nothing I haven't pointed out already.

_Posted:_ 2009/9/8 _Last modified:_ 2009/9/9



[All reviews](../Reviews/Main "Reviews:Main") | [Add a comment at the bottom of this page](index.php@title=Odp%253AAdd_comment&target=../Reviews/AlessandroAdamou_about_DisjointnessOfComplement_(DOC)).md).md).html#New_comment "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_comment&target=Reviews:AlessandroAdamou_about_DisjointnessOfComplement_(DOC)#New_comment")


Retrieved from "[http://ontologydesignpatterns.org/wiki/Reviews:AlessandroAdamou\_about\_DisjointnessOfComplement\_%28DOC%29](../Reviews/AlessandroAdamou_about_DisjointnessOfComplement_(DOC)).md).md).html)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [QCReview](../Category/QCReview "Category:QCReview")