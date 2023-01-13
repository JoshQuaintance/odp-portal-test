#  Proliferation of URIs, Managing Coreference


__Title:__ Proliferation of URIs, Managing Coreference


__Description:__ General Issue: There are some negative consequences to the current proliferation of new URIs being minted for the same things. The issue is how to avoid or manage this. 


__Diagram__
_(this article has no graphical representation)_



#  About


  




#  Additional information


##  Concise Summary


_Issue_: How to avoid or manage two negative consequences to the current proliferation of new URIs being minted for the same things. Specifically: 



1. it is hard to find when two things should be the same
2. even if you can find the links, prolific use of owl:sameAs will create computational problems.


_Source:_ This discussion is taken from a thread called [Managing Co-reference (Was: A Semantic Elephant?)](http://lists.w3.org/Archives/Public/semantic-web/2008May/0081.html "http://lists.w3.org/Archives/Public/semantic-web/2008May/0081.html") on the [W3C Semantic Web Discussion List](http://lists.w3.org/Archives/Public/semantic-web/ "http://lists.w3.org/Archives/Public/semantic-web/"). A vigorous discussion initially took place off the list, and then was moved to the list for the record. 


_Related Discussions_: [URIs and Unique IDs](http://lists.w3.org/Archives/Public/semantic-web/2008Oct/0192.html "http://lists.w3.org/Archives/Public/semantic-web/2008Oct/0192.html")


_Related Modeling Issues:_



* [Overloading OWL sameAs](../Community/Overloading_OWL_sameAs "Community:Overloading OWL sameAs")
* [Versioning and URIs](../Community/Versioning_and_URIs "Community:Versioning and URIs")


_Example(s)_



1. Wordnet issued new URIs for all of its terms for the new version, even when they referred to exactly the same thing.
2. Yago and DBpedia minted different URIs for the exact same Yago classes


_Conclusions:_



1. to some extent, URI proliferation is inevitable in an open web. It is probably the only way to allow people to independently publish web data.
2. We will have to rely on a combination of manual effort and sophisticated automated methods to detect clashes, and attempt to resolve them. There is a difference of opinion of how good a job automated techniques can do.
3. large scale duplication of URIs as in the case of YAGO and DBpedia, is unfortunate, but has now largely been rectified. That it happened at all is due to this all being very new.
4. it was argued that it does not matter much because noone is going to load all the triples into a one triple store. A counter argument to this is that even if you load a lot of triples into one store, the problem of inefficiency of sameAs reasoning can arise.
5. that these issues are arising at all can be seen as a good thing, insofar as it reflects that linked data is being made available and put to real use. Tim Berners-Lee notes that: "Life is, on balance, good."


  




##   Background


In May 2008, Michael Uschold kicked off a discussion with the subject "A Semantic Elephant" describing the unnecessary and costly proliferation of URIs and owl:sameAs links. This discussion evolved to be mostly about managing co-reference. Intitialy private, this discussion was moved to the [W3C Semantic Web Discussion List](http://lists.w3.org/Archives/Public/semantic-web/ "http://lists.w3.org/Archives/Public/semantic-web/") at Tim Berners-Lee's request. See: [Managing Co-reference (Was: A Semantic Elephant?)](http://lists.w3.org/Archives/Public/semantic-web/2008May/0081.html "http://lists.w3.org/Archives/Public/semantic-web/2008May/0081.html"). 


The original discussion evolved into a discussion about owl:sameAs per se, which has been a recurring topic on various lists over the years. [Aldo Gangemi provided a concise summary on May 16, 2008](http://lists.w3.org/Archives/Public/semantic-web/2008May/0126.html "http://lists.w3.org/Archives/Public/semantic-web/2008May/0126.html").


In October 2008, Uschold started a closely related discussion focused more on challenges with Versioning and URIs. It was under the subject: [URIs and Unique IDs](http://lists.w3.org/Archives/Public/semantic-web/2008Oct/0192.html "http://lists.w3.org/Archives/Public/semantic-web/2008Oct/0192.html").


From all this, Uschold teased out three distinct but closely related modeling isssues that are in this ODP Wiki:



1. [Overloading OWL sameAs](../Community/Overloading_OWL_sameAs "Community:Overloading OWL sameAs"): sameAs is being used in the linked data community in a way that is inconsistent with its semantics
2. __Proliferation of URIs, Managing Coreference__: How to avoid or manage two negative consequences to the current proliferation of new URIs being minted for the same things. Specifically:
	1. it is hard to find when two things should be the same
	2. even if you can find the links, prolific use of owl:sameAs will create computational problems.
3. [Versioning and URIs](../Community/Versioning_and_URIs "Community:Versioning and URIs"): When and whether to make new URIs for different versions of things.


  




##  Original Post


Here is the original Post by Michael Uschold in May 2008:


This message is about URI proliferation on the Semantic Web, illustrated by examples from DBpedia, YAGO and Wordnet. Consider this: 



1. The [Yago team](http://wzus.ask.com/r?t=p&d=us&s=a&c=a&l=dir&o=0&sv=0a300517&ip=48331b72&id=C70CD4877AC94DDE30A935341869788A&q=yago+wikipedia&p=1&qs=0&ac=3&g=081apnaichsczS&en=te&io=8&ep=&eo=&b=alg&bc=&br=&tp=d&ec=10&pt=Yago%20-%20A%20Core%20of%20Semantic%20Knowledge&ex=tsrc%3Dtxtx&url=&u=http://www.mpi-inf.mpg.de/%7Esuchanek/downloads/yago/ "http://wzus.ask.com/r?t=p&d=us&s=a&c=a&l=dir&o=0&sv=0a300517&ip=48331b72&id=C70CD4877AC94DDE30A935341869788A&q=yago+wikipedia&p=1&qs=0&ac=3&g=081apnaichsczS&en=te&io=8&ep=&eo=&b=alg&bc=&br=&tp=d&ec=10&pt=Yago%20-%20A%20Core%20of%20Semantic%20Knowledge&ex=tsrc%3Dtxtx&url=&u=http://www.mpi-inf.mpg.de/%7Esuchanek/downloads/yago/") ontologized a portion of the Wikipedia category hierarchy and produced a set of YagoClasses, each corresponding to exactly one WordNet synset.  Here is a sample URI:  
 [http://www.mpii.de/yago/resource/wordnet\_calculator\_102938886](http://www.mpii.de/yago/resource/wordnet_calculator_102938886 "http://www.mpii.de/yago/resource/wordnet_calculator_102938886")
2. The [DBpedians](http://dbpedia.org/ "http://dbpedia.org/") saw that it was good, so they added the Yago classes to their datasets. BUT:  Different URIs were used.  
 [http://dbpedia.org/class/yago/Calculator102938886](http://dbpedia.org/class/yago/Calculator102938886 "http://dbpedia.org/class/yago/Calculator102938886")
3. I found several URI conventions for Wordnet on the web, here are 3 (of how many?):
	1. [http://xmlns.com/wordnet/1.6/](http://xmlns.com/wordnet/1.6/ "http://xmlns.com/wordnet/1.6/")   
	 See: [http://xml.coverpages.org/CC-Metadata-spec-10b2.html](http://xml.coverpages.org/CC-Metadata-spec-10b2.html "http://xml.coverpages.org/CC-Metadata-spec-10b2.html")
	2. [http://wordnet.princeton.edu/~agraves/wordnet/0.9/](http://wordnet.princeton.edu/%7Eagraves/wordnet/0.9/ "http://wordnet.princeton.edu/%7Eagraves/wordnet/0.9/")  __See: [http://www.idealliance.org/papers/extreme/proceedings/html/2006/Freese01/EML2006Freese01.html#t4-1](http://www.idealliance.org/papers/extreme/proceedings/html/2006/Freese01/EML2006Freese01.html#t4-1 "http://www.idealliance.org/papers/extreme/proceedings/html/2006/Freese01/EML2006Freese01.html#t4-1")__
	3. [http://www.w3.org/2006/03/wn/wn20/instances/](http://www.w3.org/2006/03/wn/wn20/instances/ "http://www.w3.org/2006/03/wn/wn20/instances/")  __See: [http://www.w3.org/2006/03/wn/wn20/rdf/wordnet-frame.rdf](http://www.w3.org/2006/03/wn/wn20/rdf/wordnet-frame.rdf "http://www.w3.org/2006/03/wn/wn20/rdf/wordnet-frame.rdf")__


The synset IDs in the first two cases (hardwired into the URIs) are from version 3.0, but one has to poke around to discover that. There might be version problems too, _but that's another elephant._There are various issues here:



1. What is the true relationship between all these URIs? e.g are they identical in meaning?  In general, there is no good way to determine what this relationship is.
2. Why are there so many URIs for ostensibly the same exact thing?
3. Even if you do find out the exact semantic relationship, what is a practical way to resolve it?
	1. Using __owl:sameAs__ or __owl:equivalentClass__ may be adequate _logically,_ but IMHO, is wholly inadequate, _practically._ Adding large number of redundant triples and requiring inferencing will burden the already limited capabilities of knowledge stores at large scale.
	2. pre-processsing all the files with a script changing the URIs may be possible, but has its own issues:
		1. what URI should be the one chosen, yet a new one? That exacerbates the problem.
		2. a simple namespace prefix would be easy to deal with, but in the example above the names are also different. e.g. __wordnet\_calculator\_102938886__ vs. __Calculator102938886__  
		 Writing scripts that rely on naming conventions is dangerous. They may not be consistently applied and there may be 100s or 1000s or millions to check.
		3. The scripts have to be re-checked and revised and re-run each time a new version comes online


Specific Questions/Recommendations to the DBpedia and Yago teams: 



* would it  be possible to agree on a single URI for the Yago classes, and then use some other mechanism to go to the right URL?
* what is the proper logical relationship between the Yago classes and the wordnet synsets?
* Should they be taken as logically equivalent or merely as 'corresponding' to each other in some manner?
* Might that correspondence be expressed with a meta-level property,  (say correspondingSynset) with domain: YagoClass and range: WordNetSynset?


  



  



In summary: 


In Uschold's original post to selected individuals, it was noted that a proliferation of different URIs for the same resource was occurring, and that it was causing two specific problems:



1. it is hard to find when two things should be the same
2. even if you can find the links, prolific use of owl:sameAs will create computational problems.


  




##  Summary of Responses


_Chris Bizer:_


Problem 1 is not really so bad, for there is much matching technology is out there that can be used, albeit there will be some limits on precision. Problem 2 is not a problem either because noone is going to load everything into a single store.


  

_Frank van Harmelen_


Problem 1 is very real, but is only recently becoming a problem with the recent surge of semantic web data coming on line. Frank disagrees with Chris Bizer's optimism. Also, matching at the schema/class level is handled differently than matching instance. Frank refers to some good work going on in addressing these issues, not by matching after the fact, but by elminiting the proliferation at source.



1. [http://sindice.com/](http://sindice.com/ "http://sindice.com/")
2. [http://www.sindice.com/pdf/sindice-ijmso2008.pdf](http://www.sindice.com/pdf/sindice-ijmso2008.pdf "http://www.sindice.com/pdf/sindice-ijmso2008.pdf")
3. [http://www.okkam.org/](http://www.okkam.org/ "http://www.okkam.org/")
4. [http://www.okkam.org/IRSW2008](http://www.okkam.org/IRSW2008 "http://www.okkam.org/IRSW2008")


_Chris Bizer:_


My optimism was more about instance level identity links than at the class level. Within the LOD effort we repeatedly run into situations where it is really easy to generate owl:sameAs links based on some simple domain-dependent rules.


  

_Kinsgley Idehan_:


The URL problems are being addressed, e.g. in the UMBEL project. Wikipedia, OpenCye, WordNet and Yago Ideitifiers are being rationalized. See: [http://www.umbel.org/announcement.xhtml](http://www.umbel.org/announcement.xhtml "http://www.umbel.org/announcement.xhtml")


_Fred Giasson:_ 


There are edge cases when it is not immediately clear, even for a human, to decide what deserves a unique URI. 


  

_Jim Hendler:_ 


"So what you are really saying is scaling is a technology/research challenge now that there's much more out there. We need to go beyond just triple stores and get some fast inferencing at Web scales. Makes sense to me."


  

_Michael Uschold:_


The computational issue of owl:sameAs proliferation is a major problem, even if noone is going to load all the semantic web data into a single store. For today's triple stores that do limited inference, owl:sameAs "has a significant run time" [according to the developers of OpenLink's Virtuoso triplestore](http://docs.openlinksw.com/virtuoso/rdfsparqlrule.html#rdfsparqlruleintro "http://docs.openlinksw.com/virtuoso/rdfsparqlrule.html#rdfsparqlruleintro"). It can easily [double query times](http://www.openlinksw.com/weblog/oerling/?id=1347 "http://www.openlinksw.com/weblog/oerling/?id=1347").


Chris Bizer's remark that there is no need to worry because noone is going to load _all_ the data misses two important facts. First, companies that build and delivering software products using public data will have to bring the data they are using in house to control it. Second, you don't have to load _all_ the data before computational issues arise. Do you really think that, for example, Powerset relies on the data sitting on the DBpedia servers. Proliferation of URIs on a large scale will cause performance issues and should be avoided where possible.


  

_Soren Auer:_


Even with such proliferation, people will be able to build useful applications. Once, certain information sources are established (and for that page rank inspired data rank algorithms could be developed) - people will automatically tend to reuse established identifiers and this will counteract the proliferation.


  

_Tim Berners-Lee_


So multiple URIs for the same thing is life, a constant tradeoff, but life is, on balance good.



#  References


[Add a reference](index.php@title=Odp%253AAdd_reference&subject=Community%253AProliferation+of+URIs,+Managing+Coreference.html "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_reference&subject=Community%3AProliferation+of+URIs%2C+Managing+Coreference")



* Thread: Managing Co-reference (Was: A Semantic Elephant?) [Discussion Forum](http://lists.w3.org/Archives/Public/semantic-web/2008May/0078.html "http://lists.w3.org/Archives/Public/semantic-web/2008May/0078.html") | [reference page](../Community/References/W3C_SemWeb_Thread "Community:References/W3C SemWeb Thread")


 [List of Modeling Issues](../Community/Main "Community:Main") | [Post a new modeling issue](../Community/PostModelingIssue "Community:PostModelingIssue") | [Add a comment in the discussion page](index.php@title=Odp%253AAdd_comment&target=Community_talk%253AProliferation_of_URIs,_Managing_Coreference.html#New_comment "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_comment&target=Community_talk:Proliferation_of_URIs%2C_Managing_Coreference#New_comment")


Retrieved from "[http://ontologydesignpatterns.org/wiki/Community:Proliferation\_of\_URIs%2C\_Managing\_Coreference](../Community/Proliferation_of_URIs,_Managing_Coreference)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [ModelingIssue](../Category/ModelingIssue "Category:ModelingIssue")