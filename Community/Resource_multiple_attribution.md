#  Resource multiple attribution


__Title:__ General Issue: RDF Resource multiple attribution


__Description:__ General Issue: How to attribute a single resource with two values of the same property in one document 


__Diagram__
_(this article has no graphical representation)_



#  About


  




#  Additional information


_Issue_: How to attribute a single resource with two values of the same property in one document


_Example:_ publishing multiple licenses along with one rdf document. 


_Source_: The thread: [attaching multiple licenses](http://lists.w3.org/Archives/Public/public-lod/2009Dec/0046.html "http://lists.w3.org/Archives/Public/public-lod/2009Dec/0046.html") ([Markmail](http://markmail.org/thread/xu4hywhgexdmrzje "http://markmail.org/thread/xu4hywhgexdmrzje")) in the [W3C Linked Open Data Discussion List.](http://lists.w3.org/Archives/Public/public-lod/ "http://lists.w3.org/Archives/Public/public-lod/")


_Conclusions:_



1. One way is to use RDF reification, but this has some issues.
2. OWL 2 has Axiom Annotations designed to do this.
3. Caution: approaches often won't work unless the community adopts conventions and follows them.
4. Principles:
	1. two documents about the same resource should serve the same data
	2. data should not be replicated all over the place


  

_Georgi Kobilarov_ posed the [original question](http://markmail.org/message/xu4hywhgexdmrzje "http://markmail.org/message/xu4hywhgexdmrzje"): 


I'm looking for a best practice for publishing multiple licenses along with one rdf document. Say I publish one URI for an artist: [http://example.org/resource/Madonna](http://example.org/resource/Madonna "http://example.org/resource/Madonna"). 
I aggregate information from multiple sources about that artist, and those sources have different licenses. One triple comes from a source under GNU FDL, another triple from a source under Public Domain, and a owl:sameas link which I want to publish under Creative Commons License. 


Any pointers to how to do that?


  

_Toby Inkster_ [suggests](http://markmail.org/message/y65ytyk7iyus5mix "http://markmail.org/message/y65ytyk7iyus5mix") two options. One is reification, where you could create a statement resource which has the usual subject, predicate and object properties and an additional one for the licence. The other is to publish your data in a format that can make use of multiple graphs (e.g. N3). Unfortunately, this is not well supported in triple-consuming software.


However, you can fake named graphs in RDF/XML and Turtle, for example, by splitting the data into multiple documents and use rdfs:seeAlso links between the files to enable auto-dicovery. You could also duplicate that data - but that introduces other problems.


  

_Georgi Kobilarov_ [responds that](http://markmail.org/message/vi3wyhfqwk6d7qxj "http://markmail.org/message/vi3wyhfqwk6d7qxj") this solution would run into the issue that "two documents about the same resource should serve the same data". The html output would probably show all triples, but the content negotiated / 303ed rdf document would contain only links to other rdf documents. This would have to be set as common practice for it to work.


  

_Tom Heath_ [suggests](http://markmail.org/message/i5stbltaiajlvpip "http://markmail.org/message/i5stbltaiajlvpip") including the triples by reference to the source documents, rather than replicating external triples. In his view, "there's something that feels fundamentally wrong about replicating RDF data rather than just pointing applications to the places where they can find it... [it] seems fundamentally un-Web-like"


  

_Alan Ruttenberg_ [points out that](http://markmail.org/message/p2r4ne6woyoxr6ip "http://markmail.org/message/p2r4ne6woyoxr6ip") OWL 2 provides a documented way of doing this using [Axiom Annotations](http://www.w3.org/TR/2009/REC-owl2-syntax-20091027/#Annotations "http://www.w3.org/TR/2009/REC-owl2-syntax-20091027/#Annotations") along with a mechanism for [translating axioms with annotations](http://www.w3.org/TR/2009/REC-owl2-mapping-to-rdf-20091027/#Translation_of_Axioms_with_Annotations "http://www.w3.org/TR/2009/REC-owl2-mapping-to-rdf-20091027/#Translation_of_Axioms_with_Annotations"). It will last, and avoids confusion caused by RDF reification.


  

_Keith Alexander_ [adds](http://markmail.org/message/tr3riemv72ujlbif "http://markmail.org/message/tr3riemv72ujlbif"): I think that any publishers of linked data that want to place some restrictions on how their data is reused, should provide clearer guidelines on the technical solutions to fulfilling those requirements. Maybe if they thought about it and realised how confusing it all is, they'd decide they didn't really want to restrict reuse that much in the first place.



#  References


[Add a reference](index.php@title=Odp%253AAdd_reference&subject=Community%253AResource+multiple+attribution.html "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_reference&subject=Community%3AResource+multiple+attribution")


  




 [List of Modeling Issues](../Community/Main.md "Community:Main") | [Post a new modeling issue](../Community/PostModelingIssue.md "Community:PostModelingIssue") | [Add a comment in the discussion page](index.php@title=Odp%253AAdd_comment&target=Community_talk%253AResource_multiple_attribution.html#New_comment "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_comment&target=Community_talk:Resource_multiple_attribution#New_comment")


Retrieved from "[http://ontologydesignpatterns.org/wiki/Community:Resource\_multiple\_attribution](../Community/Resource_multiple_attribution.md)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [ModelingIssue](../Category/ModelingIssue.md "Category:ModelingIssue")