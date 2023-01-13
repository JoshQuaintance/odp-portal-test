[![](../images/thumb/2/29/Reviewer.png/48px-Reviewer.png)](../Image/Reviewer.png "Reviewer.png")
__[TimLebo](../User/TimLebo "User:TimLebo") about [LicenseLinkedDataResources](../Submissions/LicenseLinkedDataResources "Submissions:LicenseLinkedDataResources") (Revision ID: [11654](../Submissions/LicenseLinkedDataResources@oldid=11654 "http://ontologydesignpatterns.org/wiki/Submissions:LicenseLinkedDataResources?oldid=11654"))__
Overall suggestion (score): 0 - needs major revision




 __Review Summary:__ There is currently no good solution to describe how information resources on the web can be used by the variety of consumers that may or may not be able to use them in certain ways.
The LLDR pattern proposes to describe what rights certain agents have to perform certain acts on linked data resources (datasets, statements).


The pattern incorporates some terms from existing popular vocabularies (DCTerms, VoID, CC, FOAF, ACL), but the "core three" properties hasObject, hasRight, hasSubject are too poorly defined to inspire adoption.


Besides some practical issues such as comments in the ontology, inconsistent namespacing, lack of resolvability, and prefix ambiguity and confusion, this pattern should be revised to adopt one of two perspectives:



* Use OWL to do reasoning (instead of just specifying the structure)
* Use the Directed Qualification Pattern (instead of the more ambiguous n-ary pattern)


These two are described in more detail below.
__Reviewer Confidence:__ Have reviewed hundreds of OWL ontologies and adopt portions in dozens of Linked Data modeling projects.
__Problems:__ 6) Classes versus instances (and punning)
Why does the LLDR ontology have an exemplar instance for each subclass of LinkedDataRight? When does one refer to the instance, and when does one refer to the class? When does one instantiate their own instance of the LLDR subclasses of LinkedDataRight? It would seem to me that an instance of Access is a particular occurrence of Access (say, when I downloaded your OWL file). If I did it again, I'd have another distinct instance of Access. See "Consideration of W3C PROV" for the intrinsic parallels between being permitted to do something and actually doing it (in this case, the subclasses of LinkedDataRight are prov:Activities).


  

9) Prefixes and namespaces


The prefix "lldr" was not defined in the paper, nor at prefix.cc. I've since added it to prefix.cc/lldr. [http://purl.oclc.org/NET/lldr/ns#](http://purl.oclc.org/NET/lldr/ns# "http://purl.oclc.org/NET/lldr/ns#")


The paper did not define the prefix "gr", which was fortunately defined at [http://prefix.cc/gr](http://prefix.cc/gr "http://prefix.cc/gr").
The properties "hasCurrency" and "hasCurrencyValue" in the example did not have prefixes, so I had to presume they were Good Relations properties.


The namespaces in the OWL representation seem to be inconsistent. In the paper, the following classes use the same prefix, but they do not share the same namespace ([http://purl.oclc.org/LinkedDataResource](http://purl.oclc.org/LinkedDataResource "http://purl.oclc.org/LinkedDataResource"), [http://purl.oclc.org/NET/lldr#LinkedDataRight](http://purl.oclc.org/NET/lldr#LinkedDataRight "http://purl.oclc.org/NET/lldr#LinkedDataRight")).


10) Resolvability


The following URIs are mentioned in the OWL representation but do not resolve (they 404)


[http://purl.oclc.org/access](http://purl.oclc.org/access "http://purl.oclc.org/access")
[http://purl.oclc.org/Authorisation](http://purl.oclc.org/Authorisation "http://purl.oclc.org/Authorisation")
[http://purl.oclc.org/Contract](http://purl.oclc.org/Contract "http://purl.oclc.org/Contract")
[http://purl.oclc.org/derivativeWorks](http://purl.oclc.org/derivativeWorks "http://purl.oclc.org/derivativeWorks")
[http://purl.oclc.org/distribution](http://purl.oclc.org/distribution "http://purl.oclc.org/distribution")
[http://purl.oclc.org/extraction](http://purl.oclc.org/extraction "http://purl.oclc.org/extraction")
[http://purl.oclc.org/License](http://purl.oclc.org/License "http://purl.oclc.org/License")
[http://purl.oclc.org/LinkedDataResource](http://purl.oclc.org/LinkedDataResource "http://purl.oclc.org/LinkedDataResource")
[http://purl.oclc.org/NET/lldr](http://purl.oclc.org/NET/lldr "http://purl.oclc.org/NET/lldr")
[http://purl.oclc.org/Proposition](http://purl.oclc.org/Proposition "http://purl.oclc.org/Proposition")
[http://purl.oclc.org/reproduction](http://purl.oclc.org/reproduction "http://purl.oclc.org/reproduction")
[http://purl.oclc.org/reutilization](http://purl.oclc.org/reutilization "http://purl.oclc.org/reutilization")



[http://purl.oclc.org/SimpleLicense](http://purl.oclc.org/SimpleLicense "http://purl.oclc.org/SimpleLicense")
__Community Relevance:__ I am not familiar with the licensing community, but as a member of the LInked Data community, I would say this pattern is intended to be relevant but its current design does not inspire confidence to adopt it.
__Relation to Best Practices:__ 4) Consideration of W3C PROV
After asserting some LLDR, a natural question to ask is "did anyone violate some rights?". The only way to answer that is to know what happened. The proposed pattern offers how to model what \*can\* or \*can not\* happen, but a natural and necessary complement is to also model what \*happened\*. Within Linked Data, the ontology to model what happened is undoubtedly W3C's PROV Recommendation. While one could claim that PROV integration with LLDR is "future work", would it not be better to phrase LLDR in terms of PROV in the first place, so that rights violation would be a simple matter of querying the same concepts under some addition constrains provided by LLDR? See comment "Use of Reasoning" below.


3) Level of reuse


The proposal claims value in LLDR by its "reuse" of existing vocabularies CC, FOAF, ACL, DCTerms, and VoID.
However, it does not provide reassurance that each is being reused acceptably according to the original ontology. It also does not provide justification for why the remaining portions of the reused ontologies are not also used in this pattern.
So, I am forced to do so here to gain the confidence that I should be provided by the proposed pattern and its description.


ACL is reused by grouping acl:Access as a lldr:LinkedDataRight. But, why was acl:Authorization and acl:InformationResource not reused by LLDR? They both seem to apply to your requirements. acl:Authorization is either a subclass of lldr:RightsExpression or is equivalent. lldr:LinkedDataResources are acl:InformationResources, and the LLDR pattern should apply more generally to the latter.


CC is reused by cc:License, cc:Requirement, cc:Permission, cc:Prohibition, cc:requires, cc:Reproduction, cc:Distribution, and cc:DerivativeWorks. The ontology does not mention cc:requires, although it appears in the example in the paper. The paper diagram shows that cc:Requirement is a subclass of lldr:RightsExpression, but cc:Requirement does not appear in the OWL. The comment on lldr:Reutilization sounds a lot like its superclass cc:Distribution, what's the difference? Do cc:Reproduction,Distribution,DerivedWorks not relate to cc:Permission,Requirement,Prohibition in the CC ontology? I find it hard to believe that they'd be isolated, but cannot spend the time to dig into CC for this review. I will omit a complete comparison to CC in this review, but it should be done by the authors.


FOAF is reused by using foaf:Agent. Although this is a straight forward choice, the FOAF definition is known to have problems when using it to perform reasoning.


VoID is reused because LLDR only applies to LinkedData resources and VoID is the primary way to talk about RDF datasets. But, since LLDR is a "pattern", it should apply to any kind of information resource (like ACL's) and not just linked data.



DCTerms is reused by dcterms:license. It's not clear how this is a part of the pattern. However, if the directed qualification pattern were used, the relation between dcterms:license and a RightsExpression would make perfect sense. See comment "Qualification pattern". In this case, RightsExpression would be a subclass of rdf:Statement with restriction onProp rdf:predicate value dcterms:license. With this, you'd be qualifying the license of the resource with respect to the agent, use, etc.
__Reusability:__ It is too specific to Linked Data resources when it could apply generically to any information resource. More comments below.
__Relations to Other Patterns:__ 7) Qualification pattern
It should be noted that the n-ary relation pattern is also known as the "Qualification pattern" (as discussed at [http://patterns.dataincubator.org/book/qualified-relation.html](http://patterns.dataincubator.org/book/qualified-relation.html "http://patterns.dataincubator.org/book/qualified-relation.html")). In addition, an emerging "triple-oriented" qualification pattern can be seen as a more natural n-ary relation modeling for Linked Data and the semantic web, since the relation class is implicitly reifying a particular triple instead of just "wrapping a bunch of resources" into a single ambiguous relationship. This pattern can be seen for arbitrary properties in SIO ([https://code.google.com/p/semanticscience/wiki/SIO](https://code.google.com/p/semanticscience/wiki/SIO "https://code.google.com/p/semanticscience/wiki/SIO") - sio:has-attribute, sio:Attribute, sio:refers-to) and for particular properties in W3C PROV-O (prov:qualified\*, prov:Influence, prov:{entity, agent, activity}).
__Overall Understandability:__ 2) Definitions of new concepts
The primary terms lldr:RightsExpression, lldr:LinkedDataResource, lldr:LinkedDataRight, lldr:hasSubject, lldr:hasRight, and lldr:hasObject are not given a natural language definition in the paper.


While RightsExpression is given a good natural language definition in the OWL representation, and lldr:LinkedDataResource and lldr:LinkedDataRight are self-explanatory, the peculiar properties lldr:hasSubject, lldr:hasRight, and lldr:hasObject do not have any natural language comments. These three properties are by far the weakest part of the pattern because they are so poorly defined; they seem only to be "defined by example." And, unfortunately, they are the crux of the pattern. See comments "Use of Reasoning" and "No concrete examples" below.


Looking at the subclasses of lldr:LinkedDataRight, what is "Linked Data" about it? It appears as though it should be more generally named lldr:Right, which would parallel your lldr: RightsExpression much more naturally and permit application to resources beyond your lldr:LinkedDataResources.


Does the diamond in the UML diagram between RightsExpression and License/Contract indicate aggregation? Nothing is defined in the OWL representation except for a subclass relationship. This seems to be contradictory.


  



12) Approachability for a licensing novice



The pattern proposal and description does not provide enough background information about the licensing domain to enable an expert OWL and Linked Data developer to apply the concept. Granted, licensing is a challenging topic, but the pattern should include at least a primer and pointers to authoritative resources that outline the challenges and best practices for licensing practitioners.
__Clear Problem Description:__ The problem description was very broadly stated, and the "definition by examples" were insufficient to clearly show how they addressed each of objectives stated.
__Clear Relevance and Consequences:__ 8) Use of reasoning
Despite being a submission to the Ontology Patterns community, the LLDR proposal does not use any "useful" inference. The only inferences that are used define the structure that should be followed for assertion (and even that is incomplete and not usable). OWL allows us to share domain knowledge by exchanging domain-independent axioms that permit a non expert to determine what inferences can and should be applied to understand the domain. This is not the case for LLDR. The proposal provides merely terms and does not leverage any OWL reasoning to facilitate the understanding of the domain it is modeling. For example, "can not be used" is expressed in OWL using a restriction such as "max 0 on prov:used" and "obligated" is an inference in the form "If one does X, Y must also occur". This can be modeled in OWL, but I'm not going to provide the solution in this review. A satisfying solution for modeling the License of Linked Data Resources would be to provide axioms over the PROV notions of Agents, the kinds of Activities they perform (such as Distributing), and their use and generation of Entities (Works, Licenses, etc). See comment "Approachability for a licensing novice" below.
__Clear Figures and Illustrations:__ Does the diamond in the UML diagram between RightsExpression and License/Contract indicate aggregation? Nothing is defined in the OWL representation except for a subclass relationship. This seems to be contradictory.
The paper did not define the prefix "gr", which was fortunately defined at [http://prefix.cc/gr](http://prefix.cc/gr "http://prefix.cc/gr").
The properties "hasCurrency" and "hasCurrencyValue" in the example did not have prefixes, so I had to presume they were Good Relations properties.



The namespaces in the OWL representation seem to be inconsistent. In the paper, the following classes use the same prefix, but they do not share the same namespace ([http://purl.oclc.org/LinkedDataResource](http://purl.oclc.org/LinkedDataResource "http://purl.oclc.org/LinkedDataResource"), [http://purl.oclc.org/NET/lldr#LinkedDataRight](http://purl.oclc.org/NET/lldr#LinkedDataRight "http://purl.oclc.org/NET/lldr#LinkedDataRight")).
__Missing Information:__ 1) Compared to related RELs
The paper claims that the proposed pattern is conceived by extracting commonalities among the well-known Rights Expression Languages, but does not provide even a sketch of the mapping between the proposed pattern and the essential concepts in each of these other languages. In addition, the paper does not indicate the shortcomings of the well-known RELs or the advantages that the LLDR pattern provides. Why not just use the existing and well-known languages?


5) Relationship to Planning


The research topic of AI planning centers around conditions and consequences, and seems to be extremely relevant to your concepts and requirements. The LLDR ontology should be compared and contrasted with this body or related work.


11) No concrete examples



There should be concrete RDF/OWL examples available to illustrate \*each\* term proposed in the ontology. There are no examples provided. Beyond examples for illustration, where are the real examples of this pattern being used in the wild? In Linked Data, that should be easy to fulfill, since it can just be done and one can point to them. If there hasn't been a need compelling enough to actually solve a real problem, then is the pattern truly simple, useful, and worthwhile enough for others to adopt?

_Posted:_ 2013/8/2 _Last modified:_ 2013/8/2



[All reviews](../Reviews/Main "Reviews:Main") | [Add a comment at the bottom of this page](index.php@title=Odp%253AAdd_comment&target=../Reviews/TimLebo_about_LicenseLinkedDataResources#New_comment "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_comment&target=Reviews:TimLebo_about_LicenseLinkedDataResources#New_comment")


Retrieved from "[http://ontologydesignpatterns.org/wiki/Reviews:TimLebo\_about\_LicenseLinkedDataResources](../Reviews/TimLebo_about_LicenseLinkedDataResources)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [QCReview](../Category/QCReview "Category:QCReview")