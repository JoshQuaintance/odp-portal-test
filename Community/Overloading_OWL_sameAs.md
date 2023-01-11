#  Overloading OWL sameAs


__Title:__ General Issue: Overloading of owl:sameAs


__Description:__ General Issue: owl:sameAs is being used in the linked data community in a way that is inconsistent with its semantics. 


__Diagram__
_(this article has no graphical representation)_



#  About


  




#  Additional information


##   Concise Summary


_Issue:_ owl:sameAs is being used in the linked data community in a way that is inconsistent with its semantics. 


_Source_: Numerous, this issue has been discussed over and over on various lists. The summary so far is mainly based on a discussion that was originally about the proliferation of URIs and managing co-reference, and evolved into a discussion about owl:sameAs _per se_. 



* [W3C Semantic Web List](http://lists.w3.org/Archives/Public/semantic-web/ "http://lists.w3.org/Archives/Public/semantic-web/"): [Managing Co-reference (Was: A Semantic Elephant?)](http://lists.w3.org/Archives/Public/semantic-web/2008May/0126.html "http://lists.w3.org/Archives/Public/semantic-web/2008May/0126.html") May 2008
* [W3C Semantic Web List](http://lists.w3.org/Archives/Public/semantic-web/ "http://lists.w3.org/Archives/Public/semantic-web/"): [ISBNs, owl:sameAs, etc](http://lists.w3.org/Archives/Public/semantic-web/ "http://lists.w3.org/Archives/Public/semantic-web/") December 2009


_Related Discussions:_ 



* [linking open data] [Open Data&msgId=19328 URI aliases and owl:sameAs was: Terminology Question](http://simile.mit.edu/mail/ReadMsg?listName=Linking "http://simile.mit.edu/mail/ReadMsg?listName=Linking")


* W3C public-lod [sameAs proliferation (was Visualizing LOD Linkage)](http://www.mail-archive.com/public-lod@w3.org/msg00663.html "http://www.mail-archive.com/public-lod@w3.org/msg00663.html") August 2008
* W3C public-lod [owl:sameAs links from OpenCyc to WordNet](http://lists.w3.org/Archives/Public/public-lod/2009Feb/0186.html "http://lists.w3.org/Archives/Public/public-lod/2009Feb/0186.html") February 2009
* W3C semantic-web-lifesci [owl:sameAs and identity [was Re: blog: semantic dissonance in uniprot](http://lists.w3.org/Archives/Public/public-semweb-lifesci/2009Mar/0169.html "http://lists.w3.org/Archives/Public/public-semweb-lifesci/2009Mar/0169.html")] March 2009
* [[tbc-users](http://www.mail-archive.com/topbraid-composer-users@googlegroups.com/msg00994.html "http://www.mail-archive.com/topbraid-composer-users@googlegroups.com/msg00994.html") counting and owl:sameAs] April 2009
* W3C public-lod [how do I report bad sameAs links? (dbpedia <-> Cyc)](http://lists.w3.org/Archives/Public/public-lod/2009Jun/0443.html "http://lists.w3.org/Archives/Public/public-lod/2009Jun/0443.html") June 2009
* W3C public-lod [sameas.org](http://lists.w3.org/Archives/Public/public-lod/2009Jun/0038.html "http://lists.w3.org/Archives/Public/public-lod/2009Jun/0038.html") June 2009
* W3C public-lod [A "sameas" widget for Firefox](http://www.mail-archive.com/public-lod@w3.org/msg02554.html "http://www.mail-archive.com/public-lod@w3.org/msg02554.html") June 2009
* W3C public-lod [owl:sameAs [recipe](http://lists.w3.org/Archives/Public/public-lod/2009Jul/0306.html "http://lists.w3.org/Archives/Public/public-lod/2009Jul/0306.html")] July 2009
* W3C public-lod [SKOS, owl:sameAs and DBpedia](http://lists.w3.org/Archives/Public/public-lod/2010Mar/0215.html "http://lists.w3.org/Archives/Public/public-lod/2010Mar/0215.html") March 2010


_Related Modeling Issues_: 



* [Versioning and URIs](../Community/Versioning_and_URIs.md "Community:Versioning and URIs")
* [Proliferation of URIs, Managing Coreference](../Community/Proliferation_of_URIs,_Managing_Coreference.md "Community:Proliferation of URIs, Managing Coreference")


_Examples:_



* relating a foaf:Person instance to the person's home page.
* relating a geographical region with a political entity. For example, the physical area that a city occupies with the city itself.
* relating the DBpedia resource referring to a place with to a GeoNames resource corresponding to that same place


_Conclusions:_


There is a lot of confusion about how owl:sameAs should be used in the linked open data community. It is being used in ways that are semantically incorrect and can give incorrect inferences. A number of points and suggestions came up.



1. There is frequent tendency to use sameAs to link resources that provide information about something to resources that represent the thing. E.g. relating a resource denoting a book to a resource that is the Amazon page for the book.
2. There is a tradeoff between formal accuracy on the one hand and pragmatic usefulness on the other hand. It often arises that treating things as the same has the desired behavior. Rather than being harmful, the vagueness can be an advantage.
3. It was proposed that a weaker similarity relationship be created to be used instead of sameAs when there is not true identity between the two resources. Some argued that there already are alternatives, e.g. skos:related and rdfs:seeAlso
4. Arguments were given pro and con, as to whether the new relationship should have a formal semantics. One proposal creates a mechanism that removes it from the logic entirely See: [Managing URI Synonymity to Enable Consistent Reference on the Semantic Web](http://eprints.ecs.soton.ac.uk/15614/1/camera-ready.pdf "http://eprints.ecs.soton.ac.uk/15614/1/camera-ready.pdf"). If the formal semantics is important, should the similarity relation
	1. be a relation in the logical vocabulary of OWL, as sameAs is? -or-
	2. be just a relation in an ontology?
5. Having too many ways to specify similarity might be confusing and hinder uptake of the technology.
6. A suggestion was made to have owl:sameAs links made in separate files so that they can easily be excluded.
7. A suggestion was made that there be specific guidelines and practices between owners of data in how they reach agreement on what should be linked. See: [Bernard Vatant suggested some good practice of mutual linking](http://blog.hubjects.com/2007/07/using-owlsameas-in-linked-data.html "http://blog.hubjects.com/2007/07/using-owlsameas-in-linked-data.html")


  




##   Background


In May 2008, Michael Uschold kicked off a discussion with the subject "A Semantic Elephant" describing the unnecessary and costly proliferation of URIs and owl:sameAs links. This discussion evolved to be mostly about managing co-reference. Intitialy private, this discussion was moved to the [W3C Semantic Web Discussion List](http://lists.w3.org/Archives/Public/semantic-web/ "http://lists.w3.org/Archives/Public/semantic-web/") at Tim Berners-Lee's request. See: [Managing Co-reference (Was: A Semantic Elephant?)](http://lists.w3.org/Archives/Public/semantic-web/2008May/0081.html "http://lists.w3.org/Archives/Public/semantic-web/2008May/0081.html"). 


The original discussion evolved into a discussion about owl:sameAs per se, which has been a recurring topic on various lists over the years. [Aldo Gangemi provided a concise summary on May 16, 2008](http://lists.w3.org/Archives/Public/semantic-web/2008May/0126.html "http://lists.w3.org/Archives/Public/semantic-web/2008May/0126.html").


In October 2008, Uschold started a closely related discussion focused more on challenges with Versioning and URIs. It was under the subject: [URIs and Unique IDs](http://lists.w3.org/Archives/Public/semantic-web/2008Oct/0192.html "http://lists.w3.org/Archives/Public/semantic-web/2008Oct/0192.html").


From all this, Uschold teased out three distinct but closely related modeling isssues that are in this ODP Wiki:



1. __Overloading OWL sameAs__: sameAs is being used in the linked data community in a way that is inconsistent with its semantics
2. [Proliferation of URIs, Managing Coreference](../Community/Proliferation_of_URIs,_Managing_Coreference.md "Community:Proliferation of URIs, Managing Coreference"): How to avoid or manage two negative consequences to the current proliferation of new URIs being minted for the same things. Specifically:
	1. it is hard to find when two things should be the same
	2. even if you can find the links, prolific use of owl:sameAs will create computational problems.
3. [Versioning and URIs](../Community/Versioning_and_URIs.md "Community:Versioning and URIs"): When and whether to make new URIs for different versions of things.


  




##   July 2007 Thread


In July 2007, [Bernard Vatant suggested some good practice of mutual linking](http://blog.hubjects.com/2007/07/using-owlsameas-in-linked-data.html "http://blog.hubjects.com/2007/07/using-owlsameas-in-linked-data.html") _quoted below_:


It's been a very long and interesting [thread](http://simile.mit.edu/mail/BrowseList?listName=Linking%20Open%20Data&from=13231&amp;to=13231&by=thread "http://simile.mit.edu/mail/BrowseList?listName=Linking%20Open%20Data&from=13231&amp;to=13231&by=thread") on [Linking Open Data](http://universimmedia.blogspot.com/2007/02/linking-open-data.html "http://universimmedia.blogspot.com/2007/02/linking-open-data.html") forum and elsewhere, about the use and semantics of owl:sameAs. I just suggested the following best practices :



1. Assertions such as "a:foo owl:sameAs b:bar" should be grounded on some form of agreement of the owners of a:foo and b:bar, on whichever basis they both decide to agree.
2. For outsiders (owning neither a: or b: domains), such agreement could be shown by the presence of the assertion in symmetrical way in both domains, each domain using its own URI/resource on subject side, and the other's on object side, that is :(a) asserts "a:foo owl:sameAs b:bar"(b) asserts "b:bar owl:sameAs a:foo".
3. If one side (a) pushes the assertion first, the other side (b) should be at least made aware of it by (a), and is entitled to say she agrees or not : (a) says that "a:foo owl:sameAs b:bar", but as the owner of (b), I do not necessarily agree. Such lack of agreement could be implicitly entailed from the absence of the reciprocal assertion on (b) side.


Granted, from a pure logical viewpoint, those assertions are strictly equivalent since owl:sameAs is a symmetrical property, but from a social/trust viewpoint, having each side declaring it in a specific direction could be interpreted as a formal proof of agreement. It's what have been done e.g. between [DBpedia](http://dbpedia.org/resource/Berlin "http://dbpedia.org/resource/Berlin") and [GeoNames](http://sws.geonames.org/2950159/ "http://sws.geonames.org/2950159/"). The title thread shows once again by its sheer length, and if necessary, that there is no universal way to ground such agreement, which belongs to the realm of language and social communication. 


  




##   May 2008 Thread


In May 2008, after a vigorous discussion, [Aldo Gangemi summarized the issues on May 16, 2008](http://lists.w3.org/Archives/Public/semantic-web/2008May/0126.html "http://lists.w3.org/Archives/Public/semantic-web/2008May/0126.html") as follows:



* Issue 1: managing to suggest the rationale of owl:sameAs appropriately, i.e. in a harmless way for future usages (Aldo, Michael)
* Issue 2: distinguishing "data provision" vs. "representational" usages of owl:sameAs (Yves)
* Issue 3: need for another operator, e.g. representing equality under a closed set of properties (Geoff, Harry), or some relaxed rdfs:sameAs (Jim)
* Issue 3a: using another existing relation, such as skos:related or rdfs:seeAlso, but these are either too weak (rdfs:seeAlso), or constrained (skos:related)
* Issue 4: need for a semiotic grasp over co-reference, maybe outside formal semantics (Bernard, Peter)


On issue (1), it seems that either most people agree, or they tend to prefer a discussion on issue (2), i.e. that when data provision is the intended usage, the referential vagueness introduced by owl:sameAs in many cases is not harmful, but an advantage. As Hugh puts it: "we consider coreference as more knowledge about things, which can be represented in the SW, and can be used by applications if and when they see fit. And as someone said, there is no truth, only opinions. So we need an infrastructure for opinions, but that is the SW."


  

But at this point, others switch to issue (3), and say (including me) that, if this is the case, it would be better to choose/define a different operator that ensures a safe semantics, instead of relying on an actual identity operator like owl:sameAs. Finally, some nasty :) semioticians subtly suggest that we need some way out of formal semantics, in order to represent a kind of "similarity semantics". As Peter puts it: "Everyone talks about meaning without saying what it is they are trying to achieve by agreeing on a formal meaning".


  

My position, which I had when proposing the thread, is that we need to use things as efficiently as possible, without creating areas for useless wrong inferences. Another operator would be perfect, but (as Michael, Geoff, Harry require) it should provide the user with some serious features, comparable to what owl:sameAs does. Therefore, we need to talk about similarity, equality, etc. at the metalevel, just as owl:sameAs does, since it is a relation in the logical vocabulary of OWL, not a relation from a specific ontology. Most problems of co-referencing and identity seem to arise from the collapsing of the distinction between entities and information that denotes those entities (as noticed by Bernard, Harry, Aldo), be it dependent on some "meaning" or not. The metalevel we need to address is therefore the semiotic one, as correctly pointed in this discussion.


  

My proposal is that such metalevel is not necessarily "outside formal semantics", and some work from my group and elsewhere is proceeding in the direction of a reconciliation between a semiotic, social meaning, and the formal encoding of meaning.


  




##   Summary and Synthesis


_Correct Usages:_ A common case of a correct use is to link one resource that denotes a particular real world object to another resource that denotes the same object. Typically this will be done in two different collections of resources from two different namespaces. Examples:



* the DBpedia resource referring to a music album should have a sameAs link to a MusicBrainz resource that denotes that same album
* the DBpedia resource referring to a company should have a sameAs link to a DailyMed resource referring to that same company
* an instance of a foaf:Person denoting Tim Berners-Lee should have a sameAs link to the resource in DBLP corresponding to Tim Berners Lee.


_Possibly correct usage:_



* the DBpedia resource referring to a place may have a sameAs link to a GeoNames resource corresponding to that same place
	+ <http://dbpedia.org/resource/Bangalore> <http://www.w3.org/2002/07/owl#sameAs> <http://sws.geonames.org/1277333/> .
	+ Note that the geonames reference is to a web page, not necessarily to an RDF resource.


_Probably incorrect usages:_ 



1. relating a foaf:Person instance to the person's home pageThis should be done using the relationship: foaf:homepage, not owl:sameAs.
2. relating a resource denoting a book to a resource that is the Amazon page for the book.
3. relating a geographical region with a political entity. For example, the physical area that a city occupies with the city itself.


The first two are similar in that there is a confusion between a resource denoting a real world entity and a web page that contains information about that real world entity. 


The books example is interesting because for most intents and purposes, people just want to say: yes, the books we are talking about in each case are the same. So owl:sameAs seems highly appropriate. This likely work much of the time. It could be a problem for someone wanting to analyze an Amazon web page for say its structure and layout. Then the book that the web page is featuring is an attribute of the web page, not the web page itself.


  

_Issue:_ even if the usage is strictly incorrect, in some cases it may not matter. It depends on the intended use. Using owl:sameAs in a variety of ways with somewhat vague semantics can actually be an advantage.


We can have best of both worlds if we have a more generic relation that is being used the way owl:sameAs is now (vaguely) and having sub-relations that have more specific meanings. 


  

_Issue:_ If we move to a new vocabulary of similarity relationships that inludes the curent sameAs (as strictly defined) as well as a looser relationship (as sameAs is often used in practice), then there is a communication and migration challenge getting people to use them correctly.


Maybe what is now called â€œsameAs: should be renamed to â€œliteralSameAsâ€ and then the strictly correct uses of sameAs could be changed to literalSameAs, and the loose ones would remain the same. 


  

__Ideas / Proposals__


_More vocabulary needed to cover different cases. The vocabulary should provide clear and formal semantics, in the way that sameAs has, the semantics will be weaker._


_Essentially the same thing:_ The main thing being talked about by one resource is for all _non-technical_ intents and purposes the same thing that is being talked about by the other resource.Examples



* + DBpedia country related to the corresponding GeoNames URI.
	+ a person or company related to their home page. There already is a foaf:page relationship for this, so this could be set as a sub-property of _EssentiallyTheSameThing_
	+ A book like, On the Road and various ISBNs for various manifestations of that book.


_Use existing properties like rdfs: seeAlso and skos:related to denote similarity, which is what owl:sameAs is often used for._


This may have some merit, but often these have too weak a semantics.


  

Distinguish a set of core assertions about a resource from ancillary assertions. See: _[http://dbooth.org/2007/uri-decl/](http://dbooth.org/2007/uri-decl/ "http://dbooth.org/2007/uri-decl/")_ 


  

__Good points raised:__



* Most problems of co-referencing and identity seem to arise from the collapsing of the distinction between entities and information that denotes those entities. Thus the metalevel we need to address is the semiotic one. [Aldo's] proposal is that such metalevel is not necessarily "outside formal semantics", and some work from my group and elsewhere is proceeding in the direction of a reconciliation between a semiotic, social meaning, and the formal encoding of meaning.
* A URN and a non-URN URI can be linked by owl:sameAs. Example:urn:ietf:rfc:3187 (URN) owl:sameAs [http://tools.ietf.org/html/rfc3187.html](http://tools.ietf.org/html/rfc3187.html "http://tools.ietf.org/html/rfc3187.html") (URL).
* if too many things are sameAs to lots of other things, then the amount of intelligent conclusions you can draw from the LOD cloud will be limited. (Martin Hepp)


#  References


[Add a reference](index.php@title=Odp%253AAdd_reference&subject=Community%253AOverloading+OWL+sameAs.html "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_reference&subject=Community%3AOverloading+OWL+sameAs")



* Suggested best practice [Blog](http://blog.hubjects.com/2007/07/using-owlsameas-in-linked-data.html "http://blog.hubjects.com/2007/07/using-owlsameas-in-linked-data.html") | [reference page](../Community/References/Vatant_Blog.md "Community:References/Vatant Blog")


 [List of Modeling Issues](../Community/Main.md "Community:Main") | [Post a new modeling issue](../Community/PostModelingIssue.md "Community:PostModelingIssue") | [Add a comment in the discussion page](index.php@title=Odp%253AAdd_comment&target=Community_talk%253AOverloading_OWL_sameAs.html#New_comment "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_comment&target=Community_talk:Overloading_OWL_sameAs#New_comment")


Retrieved from "[http://ontologydesignpatterns.org/wiki/Community:Overloading\_OWL\_sameAs](../Community/Overloading_OWL_sameAs.md)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [ModelingIssue](../Category/ModelingIssue.md "Category:ModelingIssue")