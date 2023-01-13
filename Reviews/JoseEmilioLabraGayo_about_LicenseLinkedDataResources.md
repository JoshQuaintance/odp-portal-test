[![](../images/thumb/2/29/Reviewer.png/48px-Reviewer.png)](../Image/Reviewer.png.md "Reviewer.png")
__[JoseEmilioLabraGayo](../User/JoseEmilioLabraGayo.md "User:JoseEmilioLabraGayo") about [LicenseLinkedDataResources](../Submissions/LicenseLinkedDataResources.md "Submissions:LicenseLinkedDataResources") (Revision ID: [11657](../Submissions/LicenseLinkedDataResources@oldid=11657.md "http://ontologydesignpatterns.org/wiki/Submissions:LicenseLinkedDataResources?oldid=11657"))__
Overall suggestion (score): 1 - needs minor revision




 __Review Summary:__ The authors propose a pattern to assert license issues based on n-ary relations between license, action, agent, resource and condition. 
The accompanying paper contains a more detailed introduction than the web page. Although the authors don't mention if the pattern has been employed in some real scenarios.
__Reviewer Confidence:__ High
__Problems:__ The authors declare that they relate license, author, agent, resource and condition. It is not clear if condition is the same as "cc:Requirement". If it is, I would advise to clarify or to define a property "lldr:Condition". 
Although reusing existing properties can be a good practice, if those properties have different meanings, it may be better to define new properties with a more specific meaning and relate the new properties to the others.


It is not clear if the authors separate instances and classes. It is also not clear the granularity of their proposal. The goal is to add licensing information to a statement (in the PDF document they use a partial statement about google stimated stock price) or about a dataset, or both.


  




The submission does not contain OWL examples. The examples in the PDF paper are very simple.
__Community Relevance:__ The pattern can be applied to any context.
__Relation to Best Practices:__ The pattern is related with the work on Provenance. The final goal is how to add metadata information about a dataset.
Some information that would be complimentary is the time period in which that license information is valid.
__Reusability:__ I think the proposed ontology/pattern is necessary and although this proposal may still need some work, it has a lot of potential for the future of linked data adoption.
__Relations to Other Patterns:__ As I said, the pattern is related with the work that is being done in defining provenance.
It is also related with n-ary relations.
__Overall Understandability:__ The pattern lacks some fields in the description that could improve its understandability. A good set of examples and use scenarios could help its adoption.
__Clear Problem Description:__ The problem is clearly described.
__Clear Relevance and Consequences:__ This pattern or some variation of this pattern should be adopted in order for the linked data project to success.
__Clear Figures and Illustrations:__ The figures are clear. Although, it would be interesting that the authors had provided some good example.
__Missing Information:__ There is a lack of several fields in the description, specially the examples field.

_Posted:_ 2013/8/8 _Last modified:_ 2013/8/8



[All reviews](../Reviews/Main.md "Reviews:Main") | [Add a comment at the bottom of this page](index.php@title=Odp%253AAdd_comment&target=../Reviews/JoseEmilioLabraGayo_about_LicenseLinkedDataResources.md#New_comment "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_comment&target=Reviews:JoseEmilioLabraGayo_about_LicenseLinkedDataResources#New_comment")


Retrieved from "[http://ontologydesignpatterns.org/wiki/Reviews:JoseEmilioLabraGayo\_about\_LicenseLinkedDataResources](../Reviews/JoseEmilioLabraGayo_about_LicenseLinkedDataResources.md)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [QCReview](../Category/QCReview.md "Category:QCReview")