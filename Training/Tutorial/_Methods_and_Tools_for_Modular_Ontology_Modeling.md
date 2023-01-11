__Goal__:


To offer support to the ontology designers, data publishers, and software developers interested in employing semantic technologies and ontologies by presenting the state-of-the-art in terms of methods and tools, exemplifying their usage in several real-world cases.


__Brief description__


The tutorial starts with a brief introduction to ontology design and design patterns, and then introduces modeling methods and design considerations by means of examples from different domains. We will run three hands-on sessions on ontology engineering with design patterns. In each session, the participants will model ontologies that contribute to solving the problem set forth in the scenario, using different tools and techniques. Each session will begin with a short introduction to the tooling and its basic functionality, before the attendees and tutors begin to jointly develop solutions. At regular intervals throughout the sessions, the tutors will highlight observed shared challenges, recommendations on how to overcome those challenges, or other lessons learned in the process. Attendees are required to have prior knowledge of RDF and OWL.




__Resources__:


__Exercises__:
No exercises.



[Create exercise for this tutorial](http://ontologydesignpatterns.org/wiki/Special:AddData/Form:Tutorial_Exercise_Form?Exercise_Description_Template[Tutorial]=Tutorial: Methods and Tools for Modular Ontology Modeling) | [Training area](../../Training/Main.md "Training:Main")

##   Tutorial Schedule


October 8, 2018



###   Morning


1. Introduction to ODPs and first pattern examples - Pascal Hitzler (~15 mins)  
 We introduce the idea of modular ontology modeling using ODPs as templates and illustrate examples. [slides (pdf)](http://www.pascal-hitzler.de/pub2/2018-10-ISWC-tutorial-part1.pdf "http://www.pascal-hitzler.de/pub2/2018-10-ISWC-tutorial-part1.pdf")
2. Worked example: Making a modular ontology for recipes - Pascal Hitzler (~45 mins)  
 We present a worked example which progresses from a use case description to the design of the corresponding pattern-based ontology. The scenario is that of an ontology which could in principle feed a website which allows for fine-grained semantic search for cooking recipes across different recipe websites. [slides (pdf)](http://www.pascal-hitzler.de/pub2/2018-10-ISWC-tutorial-part2.pdf "http://www.pascal-hitzler.de/pub2/2018-10-ISWC-tutorial-part2.pdf") [manuscript (pdf)](http://www.pascal-hitzler.de/pub2/mom-recipes-example.pdf "http://www.pascal-hitzler.de/pub2/mom-recipes-example.pdf")
3. Worked example: design pattern use for veterinary epidemiology - Karl Hammar (~30 mins)  
 The use of ontologies and SemWeb tech for biomedical purposes is well known, but recently applications within non-human biomedicine have also been developed. In this case an example from veterinary epidemiology is presented and discussed. [Slides (pdf)](../../images/4/4e/ISWC_2018_patterns_tutorial_part_3.pdf "ISWC 2018 patterns tutorial part 3.pdf")


######   Coffee Break


1. Hands-on Session 1: OPLa, the OPLa Annotator, and SDOnt - Cogan Shimizu  
 In this section, we first describe the Ontology Design Pattern Representation Language (OPLa) and motivate its use. Having a simple and extendable representation language to indicate the relationship between patterns, especially when modularizing a pattern is critical to embracing ontology reuse. We present an annotation tool to facilitate adoption of OPLa. Finally, we present SDOnt, a new tool for generating schema diagrams from OWL files. We have seen that many OWL files on ontologydesignpatterns.org are malformed or incorrect with respect to their reference diagrams. SDOnt provides a dynamic method for incrementally generating schema diagrams during the engineering process.


###   Afternoon


1. Hands-on Session 2: OWLAx (OWL Axiomatizer) and ROWL (SWRL Rule to OWL Axiom Converter) - Md Kamruzzaman Sarker  
 In this section, attendees practise creating modular ontologies with the support of OWLAx and ROWL. Both are Protege plugins. OWLAX is graphical interface which simplifies the creation of complete axiomatizations for ontologies; in particular it helps to make sure that simple standard axioms, which are easily forgotten by the modelers, are indeed added. OWLAx furthermore makes it possible to do so using a simple interface without the need of manually adding each axiom. ROWL complements OWLAx in that it provides support for the addition of complex axioms. It uses a rule-based interface, and a published ESWC2017 paper shows that it makes addition of complex axioms quicker and less error-prone compared with using the standard Protege interface. At the beginning of the session we will give a brief introduction on the tools. Then attendees will practise creating some example ontologies. All tutors will present and available to help and guide the audience, and for answering their questions. [introduction slides (pdf)](http://daselab.cs.wright.edu/pub2/2018-10-ISWC-tutorial-part3.pdf "http://daselab.cs.wright.edu/pub2/2018-10-ISWC-tutorial-part3.pdf") [Installing OWLAx](https://dase.cs.wright.edu/content/ontology-axiomatization-support "https://dase.cs.wright.edu/content/ontology-axiomatization-support") [installing ROWL](https://dase.cs.wright.edu/content/modeling-owl-rules "https://dase.cs.wright.edu/content/modeling-owl-rules")


Feedback: [https://bit.ly/2OMu97t](https://bit.ly/2OMu97t "https://bit.ly/2OMu97t") [[1]](https://bit.ly/2OMu97t "https://bit.ly/2OMu97t")



######   Coffee Break


1. Hands-on Session 3: eXtreme Design for WebProtégé  
 This session introduces a plugin to the well-known ontology engineering environment that allows users to find, visualise, instantiate, and align ontology design patterns or templates from web repositories. [Presentation slides](../../images/d/db/20181008_-_ISWC_2018_Tutorial_-_Introduction_to_XD_and_XDP.pdf "20181008 - ISWC 2018 Tutorial - Introduction to XD and XDP.pdf"), [Tutorial overview and instructions](../../images/2/2f/2018-10-08-ISWC-Tutorial-XDP-HandsOn-Instructions.txt "2018-10-08-ISWC-Tutorial-XDP-HandsOn-Instructions.txt"), [Tutorial data](http://karlhammar.com/data/2018/10/2018-10-08-ISWC-Tutorial-XDP-HandsOn-Data.zip "http://karlhammar.com/data/2018/10/2018-10-08-ISWC-Tutorial-XDP-HandsOn-Data.zip")


##   Presenters


###   Karl Hammar


__Affiliation:__ Jönköping University, Sweden  

__Email:__ karl.hammar@ju.se  

__Web:__ [http://karlhammar.com](http://karlhammar.com "http://karlhammar.com")  

Karl received a Ph.D. at Linköping University in 2017, and is employed within the Semantic Technologies Group at Jönköping University. Karl's research focus is on developing methods and tools for finding, specializing, and combining Ontology Design Patterns, and on ascertaining which qualities and features ODPs need to display in order to support such methods and tools. Karl also manages the Software Engineering and Mobile Platforms bachelor program at Jönköping University. He has taught a number of courses in web and distributed systems development, information logistics, etc. on undergraduate and graduate levels. He has also held workshops and tutorials supporting the use of ODPs and the eXtreme Design method within several research projects, involving both academia and industry, as well as at ISWC 2016 and ESWC 2017.



###   Pascal Hitzler


__Affiliation:__ Data Semantics Lab, Wright State University, USA  

__Email:__ pascal@pascal-hitzler.de  

__Web:__ [http://www.pascal-hitzler.de](http://www.pascal-hitzler.de "http://www.pascal-hitzler.de")  

Pascal is NCR endowed Distinguished Professor, Brage Golding Distinguished Professor of Research, and Director of Data Science at the Department of Computer Science and Engineering at Wright State University in Dayton, Ohio, U.S.A. From 2004 to 2009, he was Akademischer Rat at the Institute for Applied Informatics and Formal Description Methods (AIFB) at the University of Karlsruhe in Germany, and from 2001 to 2004 he was postdoctoral researcher at the Artificial Intelligence institute at TU Dresden in Germany. In 2001 he obtained a PhD in Mathematics from the National University of Ireland, University College Cork, and in 1998 a Diploma (Master equivalent) in Mathematics from the University of Tübingen in Germany. His research record lists over 400 publications in such diverse areas as semantic web, neural-symbolic integration, knowledge representation and reasoning, machine learning, denotational semantics, and set-theoretic topology. He is Editor-in-chief of the Semantic Web journal by IOS Press, and of the IOS Press book series Studies on the Semantic Web. For more information, see [http://www.pascal-hitzler.de](http://www.pascal-hitzler.de "http://www.pascal-hitzler.de").



###   Cogan Shimizu


__Affiliation:__ Data Semantics Lab, Wright State University, USA  

__Email:__ shimizu.5@wright.edu  

__Web:__ [http://www.coganshimizu.com](http://www.coganshimizu.com "http://www.coganshimizu.com")   

Cogan Shimizu is a PhD student at Wright State and a DAGSI (Dayton Area Graduate Studies Insitute) Fellow. His current research trajectory involves advancing the ontology engineering process with the intent to culminate in improved ontology learning techniques. To this end, he has created several tools for visualizing and explaining ODPs: OWL2DL, SDOnt, and the OPLA Annotator; these tools are to be presented at this tutorial. Additionally, in conjunction with the Battlespace Visualization Laboratory of the 711th wing of the United States Air Force, he is working on a Semantically Enhanced Visualization Framework (SEVFr).


  




###   Md Kamruzzaman Sarker


__Affiliation:__ Data Semantics Lab, Wright State University, USA  

__Email:__ sarker.3@wright.edu  

__Web:__ [http://dase.cs.wright.edu/people/kamruzzaman-sarker](http://dase.cs.wright.edu/people/kamruzzaman-sarker "http://dase.cs.wright.edu/people/kamruzzaman-sarker")  

Md Kamruzzaman Sarker is a PhD student at Wright State University. His current research focuses on making machine learning algorithms decision more transparent. Besides this he is also interested in making ontology engineering processes easier and more human friendly. For the latter he created both the OWLAx and the ROWL plugin for Protege, both of which will be presented at the tutorial. Before starting his PhD he worked in industry, at Samsung Electronics, as a software engineer.





Retrieved from "[http://ontologydesignpatterns.org/wiki/Training:Tutorial:\_Methods\_and\_Tools\_for\_Modular\_Ontology\_Modeling](../../Training/Tutorial/_Methods_and_Tools_for_Modular_Ontology_Modeling.md)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [Tutorial](../../Category/Tutorial.md "Category:Tutorial")