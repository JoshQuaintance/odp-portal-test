__Goal__:


To offer support to a continuously growing community of researchers and practitioners interested in Ontology Design patterns by way of a combination of lectures and practical work.


__Brief description__


The tutorial starts with a brief general introduction to ODPs, and then introduces modeling methodologies and design considerations by means of many examples from different domains and different perspectives. This will provides its attendees with an overview of methodological guidelines and specific techniques to effectively make them able to learn how to document, evaluate, select and reuse ODPs in their projects. Example of real use cases will be also shown and discussed; finally, a practical session using a plugin for design with ODPs will be performed, under the mentoring of the tutors. In this afternoon session, the attendees are engaged in a practical session on ODP-based design, after a brief introduction to a Protege plugin for ODP-based design that is provided for technical support. Attendees are required to have prior knowledge of RDF and OWL.




__Resources__:


__Exercises__:
No exercises.



[Create exercise for this tutorial](http://ontologydesignpatterns.org/wiki/Special:AddData/Form:Tutorial_Exercise_Form?Exercise_Description_Template[Tutorial]=Tutorial: Modular Ontology Modeling with Ontology Design Patterns at ESWC2017) | [Training area](../../Training/Main.md "Training:Main")

##   Tutorial Schedule


###   Morning


1. Introduction to ODPs and first pattern examples - Pascal Hitzler (~15 mins)  
 We briefly introduce the idea of modular ontology modeling using ODPs as templates, driven by first, simple examples. ([pdf](http://daselab.cs.wright.edu/pub2/2017-05-ESWC-Tutorial-Hitzler-Part-1.pdf "http://daselab.cs.wright.edu/pub2/2017-05-ESWC-Tutorial-Hitzler-Part-1.pdf"))
2. Some patterns and their use in the chess ontology - Pascal Hitzler (~45 mins)  
 We present a worked example which progresses from a use case description to the design of the corresponding pattern-based ontology. The example is taken from recent work (published e.g. at the COLD 2015 workshop) regarding the usefulness of ontology design patterns for linked data publishing. The scenario is that of chess data on the web; a website accompanies this part of the tutorial. ([pdf](http://daselab.cs.wright.edu/pub2/2017-05-ESWC-Tutorial-Hitzler-Part-2.pdf "http://daselab.cs.wright.edu/pub2/2017-05-ESWC-Tutorial-Hitzler-Part-2.pdf"))
3. OntoPedigree ODP for supply chains - Monika Solanki (~30 mins)  
 The sharing of product and process information plays a central role in coordinating supply chains operations and is a key driver for their success. ``Linked pedigrees _- linked datasets, that encapsulate event based traceability information of artifacts as they move along the supply chain, provide a scalable mechanism to record and facilitate the sharing of track and trace knowledge among supply chain partners. We present ``OntoPedigree_ a content ontology design pattern for the representation of linked pedigrees, that can be specialised and extended to define domain specific traceability ontologies. Events captured within the pedigrees are specified using EPCIS - a GS1 standard for the specification of traceability information within and across enterprises, while certification information is described using PROV - a vocabulary for modelling provenance of resources. We exemplify the utility of OntoPedigree in linked pedigrees generated for supply chains within the perishable goods and pharmaceuticals sectors. [(Slides)](https://drive.google.com/file/d/0B9v95zXbzVdfaDcyWE0wd0JvMk0/view?usp=sharing "https://drive.google.com/file/d/0B9v95zXbzVdfaDcyWE0wd0JvMk0/view?usp=sharing")
4. Coffee Break
5. Modular Ontology Design and Use Case: The GeoLink Example - Pascal Hitzler (~60 min)  
 We present the GeoLink Modular Ontology which was designed from first principles, using ontology design patterns, in collaboration with geo- and ocean scientists as part of the NSF EarthCube project GeoLink. The ontology is used by major U.S. ocean science data repositories for exposing and integrating their data. In addition to presenting the ontology, we will also discuss structural patterns which are helpful for the practice of ontology use and maintenance, such as shortcuts, views, and typecasting. ([pdf](http://daselab.cs.wright.edu/pub2/2017-05-ESWC-Tutorial-Hitzler-Part-3.pdf "http://daselab.cs.wright.edu/pub2/2017-05-ESWC-Tutorial-Hitzler-Part-3.pdf"))
6. The Reporting Event ODP - Agnieszka Lawrynowicz (~30 min)  
 We present the Reporting Event ODP which was designed for modelling events as elements of discourse. Information provided about an event is not treated as universal truth, but rather as a statement of a particular agent, based on defined sources - a view of an actual event. We demonstrate how this pattern can be used for modeling historical debates and events in mass media. While presenting the pattern we will also discuss some patterns re-used by the Reporting Event ODP such as the Intention Extension ODP and the Time-indexed Situation ODP. [pdf](http://www.cs.put.poznan.pl/alawrynowicz/ESWC_2017_ModularOntologies_lawrynowicz-kowalczuk.pdf "http://www.cs.put.poznan.pl/alawrynowicz/ESWC_2017_ModularOntologies_lawrynowicz-kowalczuk.pdf")


###   Afternoon


1. Intro to WebProtégé XDP plugin - Karl Hammar (~30 min)  
 XDP is a fork of WebProtégé that supports three main ODP usage steps: finding a suitable ODP, specialising that ODP for a particular modelling scenario, and aligning the resulting ODP specialisation with an existing ontology or ontology module. This section introduces XDP and demos its core functionality. [PDF](../../images/7/75/2017-05-28-ESWC-Tutorial-Hammar.pdf "2017-05-28-ESWC-Tutorial-Hammar.pdf")
2. Hands-on - Karl Hammar; all tutors available for support (~2h30mins)  
 In this section, attendees practice creating an ontology by reusing ODPs with the support of XDP, starting from a set of requirements. They go through the whole process of pattern-based ontology design. All tutors are present and available to help them in working out their exercise and for answering to their questions. [Tutorial overview and instructions](../../images/d/d6/2017-05-28-ESWC-Tutorial-HandsOn-Instructions.txt "2017-05-28-ESWC-Tutorial-HandsOn-Instructions.txt"), [Tutorial data](http://karlhammar.com/ontologies/2017/05/2017-05-28-ESWC-Tutorial-HandsOn-Data.zip "http://karlhammar.com/ontologies/2017/05/2017-05-28-ESWC-Tutorial-HandsOn-Data.zip")


##   Presenters


###   Karl Hammar


__Affiliation:__ School of Engineering, Jönköping University; Department of Computer and Information Science, Linköping University, Sweden  

__Email:__ karl@karlhammar.com  

__Web:__ [http://www.karlhammar.com](http://www.karlhammar.com "http://www.karlhammar.com")  

Karl is pursuing a Ph.D. at Linköping University, and is employed within the Semantic Technologies research group at Jönköping University. Karl's research focus is on developing methods and tools for finding, specializing, and combining Ontology Design Patterns, and on ascertaining which qualities and features ODPs need to display in order to support such methods and tools. Karl also manages the Software Engineering and Mobile Platforms bachelor program at Jönköping University. He has taught a number of courses in web and distributed systems development, information logistics, etc. on undergraduate and graduate levels. He has also held workshops and tutorials supporting the use of ODPs and the eXtreme Design method within several research projects, involving both academia and industry.



###   Pascal Hitzler


__Affiliation:__ Data Semantics Lab, Wright State University, USA  

__Email:__ pascal.hitzler@wright.edu  

__Web:__ [http://www.pascal-hitzler.de](http://www.pascal-hitzler.de "http://www.pascal-hitzler.de")  

Pascal is endowed NCR Distinguished Professor and Director of Data Science at the Department of Computer Science and Engineering at Wright State University in Dayton, Ohio, U.S.A. From 2004 to 2009, he was Akademischer Rat at the Institute for Applied Informatics and Formal Description Methods (AIFB) at the University of Karlsruhe in Germany, and from 2001 to 2004 he was postdoctoral researcher at the Artificial Intelligence institute at TU Dresden in Germany. In 2001 he obtained a PhD in Mathematics from the National University of Ireland, University College Cork, and in 1998 a Diploma (Master equivalent) in Mathematics from the University of Tübingen in Germany. His research record lists over 300 publications in such diverse areas as semantic web, neural-symbolic integration, knowledge representation and reasoning, machine learning, denotational semantics, and set-theoretic topology. He is Editor-in-chief of the Semantic Web journal by IOS Press, and of the IOS Press book series Studies on the Semantic Web. He is co-author of the W3C Recommendation OWL 2 Primer, and of the book Foundations of Semantic Web Technologies by CRC Press, 2010 which was named as one out of seven Outstanding Academic Titles 2010 in Information and Computer Science by the American Library Association's Choice Magazine, and has translations into German and Chinese. He is on the editorial board of several journals and book series and on the steering committee of the RR conference series, the NeSy workshop series, and the newly founded Association for Ontology Design and Patterns, and he frequently acts as conference chair in various functions. Pascal is the lead editor of the 2016 IOS Press book “Ontology Engineering with Ontology Design Patterns,” and he has given many tutorials for specialized and mixed audiences, on a wide range of topics, including invited tutorials at STIDS2013, OWLED2011, GeoS2009, regular tutorials at ISWC2016, AAAI-15, ISWC2010, IJCAI-09, invited Summer School classes and lectures at the 2016 Summer School on Reasoning at UQAM, Canada, the Computational Logic Summer School in Dresden, Germany 2013, and the Reasoning Web Summer School 2011 in Galway, Ireland. For more information, see [http://www.pascal-hitzler.de](http://www.pascal-hitzler.de "http://www.pascal-hitzler.de").



###   Adila Krisnadhi


__Affiliation:__ Data Semantics Lab, Wright State University, USA  

__Email:__ krisnadhi@gmail.com  

__Web:__ [http://dase.cs.wright.edu/people/Adila-Krisnadhi](http://dase.cs.wright.edu/people/Adila-Krisnadhi "http://dase.cs.wright.edu/people/Adila-Krisnadhi")   

Adila is postdoctoral researcher at the Data Semantics Lab, Wright State University. He received his Ph.D from Wright State University in 2015 with a dissertation on ontology pattern-based data integration with an application in the ocean science domain. Following up upon that, his current research is mainly focused on the area of ontology engineering and ontology design patterns. In particular, he is interested in how modular ontologies resulted from such ontology design patterns can be effectively used to realize a flexible integration over semantically heterogeneous data coming from different repositories. Besides this line of research, he also published some work on topics related to more theoretical aspects of ontology languages and an integration between ontology and rule languages. Adila is one of the editors of the 2016 IOS Press book “Ontology Engineering with Ontology Design Patterns” and is the lead author of two tutorial chapters in this book. He also has given a tutorial on Ontology Design Pattern Driven Linked Data Publishing at the Summer Meeting of the Earth Science Information Partners (ESIP), July 2016. Aside from his current position, Adila is also affiliated with the Faculty of Computer Science, Universitas Indonesia. Adila will assist in the preparation of materials but will not himself be able to present.


  




###   Agnieszka Lawrynowicz


__Affiliation:__ Poznan University of Technology, Poland  

__Email:__ alawrynowicz@cs.put.poznan.pl  

__Web:__ [http://www.cs.put.poznan.pl/alawrynowicz](http://www.cs.put.poznan.pl/alawrynowicz "http://www.cs.put.poznan.pl/alawrynowicz")  

Agnieszka is Assistant Professor at the Institute of Computing Science at Poznan University of Technology (PUT) where she also did her Ph.D. in Computer Science (with distinction) in 2009. She also holds French-Polish DESS Certificate of Ability to Manage Companies (Poznan University of Economics & University of Rennes 1) obtained from post-graduate studies in 2003. Her research interests include artificial intelligence methods, mostly knowledge representation (ontologies), knowledge discovery and the Semantic Web. Before joining academia, she worked in industry (Empolis, Bridgestone), and also was a leader of the PUT team in R&D project for France Telecom (Orange Labs) on spoken language understanding (2011). She had an EU Marie-Curie fellowship within the PERSONET project on Web mining at the University of Ulster (2004). She was the PUT team leader in EU FP7 project e-LICO (“An e-Laboratory for Interdisciplinary Collaborative Research in Data Mining and Data-Intensive Science”) (2010-2012). She is a Laureate of the Foundation for Polish Science under the POMOST program for the project LeoLOD “Learning and Evolving Ontologies from Linked Open Data” (2013-2015). She is a member of the Polish Artificial Intelligence Society, ECCAI and IAOA. She has initiated and co-organized a series of international workshops on Inductive Reasoning and Machine Learning from the Semantic Web (IRMLeS) co-located with a major Semantic Web conference (ESWC’2009-2011). She has also served as co-organizer at several events related to knowledge engineering: co-chairing the Workshop on Ontology and Semantic Web Patterns (WOP2014, WOP2016), OWL: Experiences and Directions Workshop (OWLED 2015), machine learning tracks at the Extended Semantic Web Conference (ESWC2011,ESWC2014), and serving as the workshops chair at the ESWC2017. She has served as PC member at the major conferences and workshops related to knowledge engineering: ISWC, ESWC, EKAW, WOP, OWLED, SEMANTiCS. She is a co-chair of the W3C Machine Learning Schema Community Group.



###   Monika Solanki


__Affiliation:__ Oxford University, UK   

__Email:__ monika.solanki@cs.ox.ac.uk  

__Web:__ [http://www.monikasolanki.com](http://www.monikasolanki.com "http://www.monikasolanki.com")  

Monika is a Senior Researcher at the University of Oxford. Her current research focuses on developing unified ontological models and frameworks for aligning software and data engineering processes. Besides this, she is also interested in developing data-driven frameworks for the Internet of Things and investigating the application of blockchains to support traceability in supply chains. Her past research has focused on implementing stream processing algorithms and models for tracking and tracing in supply chains, using event based pedigrees over GS1's EPCIS standards, Semantic Web standards and Linked Data technologies. Dr Solanki has extensive experience in designing and developing ontological domain models, curating linked datasets, implementing Semantic Web applications and Web services for a number of interdisciplinary projects spanning the boundaries of Computer Science, Bioenergy, Archaeology and Plant Biology. She has developed and published several ontology design patterns such as Standard Enforcer pattern, Reactor pattern, OntoPedigree, DIO and VOIC.





Retrieved from "[http://ontologydesignpatterns.org/wiki/Training:Tutorial:\_Modular\_Ontology\_Modeling\_with\_Ontology\_Design\_Patterns\_at\_ESWC2017](../../Training/Tutorial/_Modular_Ontology_Modeling_with_Ontology_Design_Patterns_at_ESWC2017.md)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [Tutorial](../../Category/Tutorial.md "Category:Tutorial")