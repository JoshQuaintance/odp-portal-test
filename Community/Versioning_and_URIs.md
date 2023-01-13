#  Versioning and URIs


__Title:__ General Issue: Versioning and URIs


__Description:__ General Issue: When and whether to make new URIs for different versions of things. 


__Diagram__
_(this article has no graphical representation)_



#  About


  




#  Additional information


##  Concise Summary


_Issue_: When and whether to make new URIs for different versions of things.


_Source_: [URIs and Unique IDs](http://lists.w3.org/Archives/Public/semantic-web/2008Oct/0192.html "http://lists.w3.org/Archives/Public/semantic-web/2008Oct/0192.html") from [W3C Semantic Web List](http://lists.w3.org/Archives/Public/semantic-web/ "http://lists.w3.org/Archives/Public/semantic-web/")


_Related Discussions_: 



* [Managing Co-reference (Was: A Semantic Elephant?)](http://lists.w3.org/Archives/Public/semantic-web/2008May/0081.html "http://lists.w3.org/Archives/Public/semantic-web/2008May/0081.html")
* [SKOS namespace change: Issue 153](http://www.w3.org/2006/07/SWD/track/issues/153 "http://www.w3.org/2006/07/SWD/track/issues/153")


_Related Modeling Issues:_



* [Proliferation of URIs, Managing Coreference](../Community/Proliferation_of_URIs,_Managing_Coreference "Community:Proliferation of URIs, Managing Coreference")
* [Overloading OWL sameAs](../Community/Overloading_OWL_sameAs "Community:Overloading OWL sameAs")


_Examples:_



1. A new version of Wordnet used a different namespace, so there were many new URIs minted for resources that were semantically identical.
2. A new version of SKOS kept the original namespace. This resulted in changing the semantics of existing URIs.


_Conclusions:_



1. There are no guidelines for when and whether to create new URIs as ontologies evolve
2. There is no consistency in how people are approaching the problem.
3. Reasons for this are:
	1. insufficient technological infrastructure for ontology maintenance & change management
	2. URIs are overloaded
4. Approaches include:
	1. Mint new URIs even thought the semantics for most may be identical
	2. Keep URI the same for a small number of terms even though the semantics may change
	3. Use depracation for old terms, keeping the same URI
	4. Mint new URIs for only the changed terms.
5. Tradeoffs:
	1. Attractive for using the ontology for the first time. The proliferation of URIs may result in maintenance and performance issues.
	2. Attractive for using the ontology for the first time. Ontology-driven applications may break.
	3. Attractive in the case when ontologies are continuously evolving.
	4. Avoids maintenance and performance issues, ontology-driven applications will not break. Challenge is lack of infrastructural support to do this accurately and efficiently.


  




##   Background


In May 2008, Michael Uschold kicked off a discussion with the subject "A Semantic Elephant" describing the unnecessary and costly proliferation of URIs and owl:sameAs links. This discussion evolved to be mostly about managing co-reference. Intitialy private, this discussion was moved to the [W3C Semantic Web Discussion List](http://lists.w3.org/Archives/Public/semantic-web/ "http://lists.w3.org/Archives/Public/semantic-web/") at Tim Berners-Lee's request. See: [Managing Co-reference (Was: A Semantic Elephant?)](http://lists.w3.org/Archives/Public/semantic-web/2008May/0081.html "http://lists.w3.org/Archives/Public/semantic-web/2008May/0081.html"). 


The original discussion evolved into a discussion about owl:sameAs per se, which has been a recurring topic on various lists over the years. [Aldo Gangemi provided a concise summary on May 16, 2008](http://lists.w3.org/Archives/Public/semantic-web/2008May/0126.html "http://lists.w3.org/Archives/Public/semantic-web/2008May/0126.html").


In October 2008, Uschold started a closely related discussion focused more on challenges with Versioning and URIs. It was under the subject: [URIs and Unique IDs](http://lists.w3.org/Archives/Public/semantic-web/2008Oct/0192.html "http://lists.w3.org/Archives/Public/semantic-web/2008Oct/0192.html").


From all this, Uschold teased out three distinct but closely related modeling isssues that are in this ODP Wiki:



1. [Overloading OWL sameAs](../Community/Overloading_OWL_sameAs "Community:Overloading OWL sameAs"): sameAs is being used in the linked data community in a way that is inconsistent with its semantics
2. [Proliferation of URIs, Managing Coreference](../Community/Proliferation_of_URIs,_Managing_Coreference "Community:Proliferation of URIs, Managing Coreference"): How to avoid or manage two negative consequences to the current proliferation of new URIs being minted for the same things. Specifically:
	1. it is hard to find when two things should be the same
	2. even if you can find the links, prolific use of owl:sameAs will create computational problems.
3. __Versioning and URIs__: When and whether to make new URIs for different versions of things.


  




##  Original Post


Currently there is no accepted practice on how/whether to migrate to new URIs when a new version of an ontology is published. This is largely due to the fact that there is no good technology for managing versioning, and the W3C consciously (and probably sensibly) decided not to address the issue. Versioning information is meant to be placed on a version annotation.


However the current situation is like the wild West, and everyone will be doing different things, resulting in a mess.



1. Wordnet published a new version and minted all new URIs even though many or most of the entries were semantically identical.
2. The SKOS working group is currently (Oct 2008) considering the pros and cons of various options. One is to adopt all new URIs in a new namespace, just like Wordnet. Another is to keep the exact same name space, and change the semantics of a small number of terms while keeping the same URI. A third is to keep the same URI for the unchanged terms, and mint new URIs for the terms with different semantics.


This is a problem because they have no guidelines, they are basically stumbling along in the dark. I believe that this is an urgent matter that needs attention to prevent a nightmare from unfolding.


In the current state of semantic web use, it may not matter to much what choice the SKOS team chooses. This is mainly relatively few applications will be impacted, which may be due to the fact that the applications are not driven by the ontologies.


However, when usage of ontologies and ontology-driven applications becomes more mainstream, the differences could be profound. Given that this issue is intimately tied up with versioning, and that we have no good solutions yet, do we continue to throw our hands up and punt? Absolutely not, it is essential that a good precedent is set ASAP that is based on sound principles. Here is how:


_We should imagine a future where ontology versioning is handled properly and do things that are going to make things easy to migrate to that future. We don't know how the versioning black box will work, but we should be able to make some clear and definitive statements about WHAT it does._


For example, in the future, ontology-driven applications will be fairly mainstream. URIs are used as unique identifiers. When applications are driven from ontologies, then they will break if you change the semantics in mid-stream. Imagine an application that relied on the semantics of broader as it was originally specified with transitivity. They loaded data that was created using that semantics. Then the SKOS spec changes and broader is no longer transitive. New datasets are created according to this new meaning. The application loads more data. It needs to know which data is subject to transitive closure and which is not. This is impossible, if the same SKOS URI is used for versions with different semantics. They are different beasts, and thus MUST have different URIs.


Similarly, if SKOS mints a whole new namespace and changes all the URIs, the application also has a problem. It has datasets with the old URI and datasets with the new URIs. This means that the datasets will not be linked like they should, they will treat the two different URIs for the same thing as being different. If one wanted to go into OWL-Full, one can use owl:sameAs, but this is not very practical.  The only reasonable solution is to have the same URI for things with the same semantics. Thus, any ontology versioning system of the future will rely on these two principles:



1. If the semantics of a term changes, then it needs to have a new unique ID.
2. If the semantics of a term does NOT change, then it should maintain the same ID in any future versions.


If either of these two guidelines are broken, then so will the ontology-driven applications of the future. These maxims hold without exception for any standards that are formally released as standards. A question arises if we need to hold to the same standards for standards like SKOS which was never formally blessed.


  




##  Summary of Followup Discussion


_Example 1: WordNet_


The WordNet maintainers published a new version in OWL format and used a new namespace which contained the new version number in it. This means that every single resource in Wordnet now has a different URI, even though many are exactly the same as before. 


_Example 2: SKOS_


In 2008, the SKOS working group is updated the SKOS vocabulary/ontology. They have decided that two terms have the wrong semantics, and the new version will reflect the correct semantics. The majority of the terms are unchanged. They chose not to mint all new URIs, but rather to use the same URI for terms with different semantics.


_Example 3: Open Biomedical Ontologies_ 


There is an explicit policy of _not_ changing URIs as new versions of the ontology are released - for one thing that would be impractical â€“ some of them are updated daily. Rather there is a policy on deprecation - terms that are deprecated are marked as such and kept in the ontology so as not to leave dangling pointers. ([Alan Ruttenberg](http://lists.w3.org/Archives/Public/semantic-web/2008Nov/0073.html "http://lists.w3.org/Archives/Public/semantic-web/2008Nov/0073.html"))


  

_Continuous vs. Discrete Ontology Evolution_


Examples 1 and 2 relate to the case where an ontology is undergoing discrete evolution - _i.e._ a specific effort is undertaken to update the ontology resulting in a new version. Example 3 relates to a the case where an ontology is undergoing (more or less) continuous evolution - _i.e._ it is changing all the time, and no attempt is made to create and name a new version of the ontology, per se. These cases may be sufficiently different to warrant different approaches.


  

_Approaches:_



1. Mint new URIs for all terms, even when the semantics does not change (Example 1:Wordnet)
2. Keep the URIs the same but change the semantics (Example 2: SKOS)
3. Do not change URIs as new versions of the ontology are released. Depracate old terms and leave them in the ontology marked as such. (Example 3: Open Biomedical Ontologies)
4. Mint new URIs for all and only the terms whose semantics changed. In the case of SKOS, this would mean new URIs for the small number of terms that changed. The ontology would presumably also get a new URI because it changed. (No examples).


  

_Tradeoffs:_


Option 1 has the apparent advantage of starting with a clean slate, and would be attractive to anyone using the ontology for the first time. However it causes a proliferation of URIs, with consequent maintenance and performance problems. Maintenance becomes problematic because the developer of the ontology-based applications needs to carefully ensure things are in order. If they are, then owl:sameAs can be used to link the old and new URIs, which is a performance problem. 


Option 2 is also attractive to anyone who is using SKOS for the first time. However it breaks a trust in the use of a URI as a unique resource. It creates a new beast with a new semantics which should have a new name. This runs the risk of breaking applications that rely on that trust. 


Option 3: is attractive because it retains backwards compatibility, but does so at the cost of extra infrastructural support.


Option 4 is attractive to anyone who wants to do things that are 'semantically proper'. This was verified by an informal poll at ISWC-2008. I asked Aldo Gangemi, Sean Bechofer, Ian Horrocks, Jeff Pan, Peter Mika, Ora Lassila, Terri Payne, Martin Hepp, Fausto G. One of these polled nevertheless preferred option 2, believing that some practical concerns trumped the semantic ones. This option is unattractive because it seems messy to have one ontology with two namespaces. It could lead in the future to arbitrarily many namespaces for the same ontology, as it evolves over time. This could all be solved with proper change management infrastructure, as yet to be invented.


  

_Root Causes_


Basically, people often know what the right thing to do is, but it is often too easy and expedient to do the wrong thing. This is exacerbated by the lack of necessary infrastructure to do the right thing. There are some key root causes.



1. lack of a good technological infrastructure for ontology maintenance
2. lack of a good technological infrastructure for change management
3. overloading of URIs


  

_Maintenance_: Currently, URIs are not sacred, they can change at the whims of their authors/maintainers. The only way to be sure is to mint and manage your own URIs and link them to other ones as a courtesy. This leads to a proliferation of URIs.


_Change management:_ Initially, the W3C consciously (and probably sensibly) decided not to address the change management and versioning issue. A stop gap solution using annotation properties was provided instead. This is not going to be solved in the short term. 


_URI overloading:_ Take a simple example from Wordnet. The following URL is being use for the many different things: http://wordnet.princeton.edu/wordnet/v2.2/pickle. This is being used to denote the authoring organization, the name of the ontology, the version of both the ontology and the ontology term, the URL, the name of the term as well as being a unique identifier. Most of these things should be able to change, leaving the URI the same. This being a common way to do things makes it too tempting to do things the 'wrong way'.


[Alan Ruttenberg](http://lists.w3.org/Archives/Public/semantic-web/2008Nov/0073.html "http://lists.w3.org/Archives/Public/semantic-web/2008Nov/0073.html") points out that this likely contributed to the SKOS problem. The terms that changed were broader and its inverse. They are no longer transitive. If the URIs were UIDs only, then you could have simply changed the label on the old broader to _broader transitive_ and moved on. This is a key reason for a movement to use opaque numeric UIDs for concepts in the Open Biomedical Ontologies.



#  References


[Add a reference](index.php@title=Odp%253AAdd_reference&subject=Community%253AVersioning+and+URIs.html "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_reference&subject=Community%3AVersioning+and+URIs")


  




 [List of Modeling Issues](../Community/Main "Community:Main") | [Post a new modeling issue](../Community/PostModelingIssue "Community:PostModelingIssue") | [Add a comment in the discussion page](index.php@title=Odp%253AAdd_comment&target=Community_talk%253AVersioning_and_URIs.html#New_comment "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_comment&target=Community_talk:Versioning_and_URIs#New_comment")


Retrieved from "[http://ontologydesignpatterns.org/wiki/Community:Versioning\_and\_URIs](../Community/Versioning_and_URIs)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [ModelingIssue](../Category/ModelingIssue "Category:ModelingIssue")