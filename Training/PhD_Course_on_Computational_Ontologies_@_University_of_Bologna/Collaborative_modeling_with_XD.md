__Problem__:
CNR is a public research organization in Italy. It wants to build a semantic data management system for expert finding, competence and project management.




__Solutions__:



#   Guidelines


* Iteration: Pick a story among the ones with the highest priority: define the competency questions, ask the customer to feedback on the CQs you have defined, model your story by re-using content patterns and with a highly modular approach. When you finish, deliver the result to the integration pair. Start a new iteration.
* Use English for the vocabularies (though rdfs:labels in multiple languages are appreciated)
* For the base URI/default namespace of your ontologies use [http://ontologydesignpatterns.org/cpont/cnr/](http://ontologydesignpatterns.org/cpont/cnr/ "http://ontologydesignpatterns.org/cpont/cnr/")_your\_filename_.owl . It will match the physical URI of your ontology.
* Add notes to the Wiki section (this page) for your own story (you can also use the discussion/talk page if you wish). For example: if the customer clarify an issue, add the new information to the story section; if you choose among more than one modeling solution, write down the modeling issue and the rationale based on that choice you made.
* Post all Competency Questions, SPARQL queries (aka unit tests), URIs (only after the ontology is delivered) etc. on the Wiki section of your story. Integrators will add the physical URIs where they are published.
* Use Camel notation for your OWL Classes and Properties (except for the rdfs:labels).
* Use word1\_word2\_word3\_... for naming individuals.
* Deliver your ontologies __ONLY__ when: all tests are successful, competency questions and SPARQL queries are posted on the story section, annotation are complete (see below).
* Tests include: SPARQL queries and consistency checking. If integrators receive inconsistent ontologies from you, they will most likely get really angry.
* Update the status of your story. It should be one of {TBD, BEING MODELED, DELIVERED, INTEGRATED}.
* Send your modules by email to adamou[AT]cs[DOT]unibo[DOT]it (Cc presutti[AT]cs[DOT]unibo[DOT]it).
* import the cp annotation schema (if you use XD tool for annotating it is imported).
* In each produced ontology module include the following annotations: labels and comments on ontology entities, coversRequirements (the competency questions), scenarios (the story description), hasUnitTest (the SPARQL queries), isSpecializationOf (if the module specialized some content ODP). Additionally, it is recommended to include also the following annotations: hasIntent, and hasConsequences.


  




##   Notes


* 5 pairs of story designers - 1 pair of integration (composition) designers
* Start time: 10:50am
* First delivery at: 12:12pm (Story 3)
* Last delivery for first iteration at: 1:02pm
* Start time of first integration iteration: 12:25pm
* First integration release at: 1:15pm
* Stop between 1:15pm and 3:40pm


#   Stories


##   Story 1


* Priority: low
* Title: CNR structure
* Description:



```
  CNR is the major italian public research body. It is organized into “scientific units” (strutture scientifiche), 
  “management units” (strutture gestionali), and “activities” (attività). Scientific units include “departments” (dipartimenti) 
  and “institutes” (istituti). Activities include “research programs” (progetti), “thematic projects” (commesse), 
  “work packages” (moduli), and “foundational research projects” (ricerca spontanea a tema libero). 

```

* Status: being modeled
* Assigned to Pair: Basile, Bragaglia
* Competency questions:



```
1) Which are the definitions of CNR?
2) What are the main parts of CNR?
3) What are the scientific units of CNR?
4) What are the management units of CNR?
5) What are the activities of CNR?
6) What is the english name of a certain part?
7) What is the italian name of a certain part?
8) What is the english name of a certain activity?
9) What is the italian name of a certain activity?

```

  




* SPARQL queries:
* ontology URI:


##   Story 2


* Priority: low
* Title: Affiliation of researchers and institutes
* Description:



```
  ISTC (The Institute for cognitive science and technology) is affiliated to the “Humanities” department 
  and it also participates in the ICT department. Aldo Gangemi belongs to the ISTC. Institutes are affiliated to 
  only one department while they can participate in several departments. Researchers belong to one institute. 

```

* Status: done
* Assigned to Pair: Luca Iori and Gioele Barabucci
* Competency questions:
	1. To which department is a given institute affiliated?
	2. In which department does a certain institute partecipate?
	3. To which institute does a certain researcher belong?
	4. Which researchers belong to a certain institute?
* SPARQL queries:
	+ CQ 1:



```
  SELECT ?dept
  WHERE {
      ?institute depts:isAffiliatedTo ?dept .
      FILTER (?institute = :istc)
  }

```

* + CQ 2:



```
  SELECT ?dept
  WHERE {
      ?institute depts:partecipates ?dept .
      FILTER (?institute = :istc)
  }

```

* + CQ 3:



```
  SELECT ?institute
  WHERE {
      ?institute depts:hasResearcher ?person .
      FILTER (?person = :aldo_gangemi)
  }

```

* + CQ 4:



```
  SELECT ?person
  WHERE {
      ?institute depts:hasResearcher ?person .
      FILTER (?institute = :istc)
  }

```

* ontology URI:



```
  [http://ontologydesignpatterns.org/cpont/cnr/story2](http://ontologydesignpatterns.org/cpont/cnr/story2 "http://ontologydesignpatterns.org/cpont/cnr/story2")

```

##   Story 3


* Priority: high
* Title: Research products
* Description:



```
  Eva Blomqvist is one of the authors of the paper entitled “Experiments on Pattern-based Ontology Design” 
  about ontology design patterns. Researchers produce various products such as publications, patents, databases. 
  Each product has at least one author and is about a topic.

```

* Status: DELIVERED
* Assigned to Pair: Andrea Burattin and Antonio Lieto
* Competency questions:


1. Who are the authors of a product (result of research)?
2. Which is the title of a product (result of research)?
3. Which papers an author wrote?
4. Which product (result of research) a resercher produced?
5. Which are the topics of a product (result of research)?
6. Which are the possible results of research?


* SPARQL queries:
	+ CQ1



```
  SELECT ?author
  WHERE {
  	?author :isAuthorOf :experiments_on_pattern_based_design .
  }

```

* + CQ2



```
  SELECT ?title
  WHERE {
  	:experiments_on_pattern_based_design :hasTitle ?title .
  }

```

* + CQ3



```
  SELECT ?papers
  WHERE {
  	:eva_blomqvist :isAuthorOf ?papers .
  }

```

* + CQ4



```
  SELECT ?products
  WHERE {
  	:eva_blomqvist :isCreatorOf ?products .
  }

```

* + CQ5



```
  SELECT ?topics
  WHERE {
  	:experiments_on_pattern_based_design :hasTopic ?topics .
  }

```

* + CQ6



```
  SELECT ?products
  WHERE {
  	?products rdfs:subClassOf :ResearchProduct .
  }

```

* ontology URI: [http://ontologydesignpatterns.org/cpont/cnr/researchproducts.owl](http://ontologydesignpatterns.org/cpont/cnr/researchproducts.owl "http://ontologydesignpatterns.org/cpont/cnr/researchproducts.owl")


We requested to the customer if a scientific product can have one or more topics.



##   Story 4


* Priority: high
* Title: types of researchers
* Description:



```
  Aldo Gangemi works at CNR since 1990 and from 2000 as senior researcher (primo ricercatore). 
  Before that he was junior researcher (ricercatore) for six years. 

```

* Status: Delivered
* Assigned to Pair: Marcello Ceci (number 3) Lino Possamai (number 5)
* Competency questions:



```
1) In which organization is a certain person employed
2) which role was covered  by a certain person in a certain period of time
3) Which roles has been covered by a certain person in a certain organization
4) When did a certain person start/stop working in a specific role?

```

* SPARQL queries:



```
SELECT ?object2 
WHERE {
    :aldo_gangemi  situation:hasOccupation ?object .
    ?object situation:occupationStructure   ?object2 .
   ?object rdf:type :Occupation .
 }
 SELECT ?roles 
 WHERE {
	timeinterval:aldo_1994_1999 situation:timeOf ?object .
	:aldo_gangemi  situation:hasOccupation ?object .
	?object situation:occupationJob ?roles .
 }
SELECT ?roles 
WHERE {
	:aldo_gangemi  situation:hasOccupation ?object .
	?object situation:occupationJob ?roles .
 }
 SELECT ?timeStart ?timeStop
 WHERE {
	:aldo_gangemi  situation:hasOccupation ?object .
  	personJob:junior_researcher situation:jobOccupation ?object .
        ?object situation:occupationTime ?object2 .
	?object2 timeinterval:hasIntervalStartDate ?timeStart .
	?object2 timeinterval:hasIntervalEndDate ?timeStop .
 }

```

* ontology URI:



```
[http://ontologydesignpatterns.org/cpont/cnr/typesofresearchers.owl](http://ontologydesignpatterns.org/cpont/cnr/typesofresearchers.owl "http://ontologydesignpatterns.org/cpont/cnr/typesofresearchers.owl")

```

##   Story 5


* Priority: low
* Title: project participation
* Description:



```
  Alessandro Adamou is a PhD student and works on the IKS project. 
  IKS project is funded by EU and is on “Semantic Content Management Systems”.

```

* Status: DELIVERED
* Assigned to Pair: Andrea Burattin and Antonio Lieto
* Competency questions:


1. Which is the current occupation of a certain prerson?
2. On which project is a certain person involved?
3. Who is the funder of a certain project?
4. Which is the topic of a certain project?


* SPARQL queries:
	+ CQ1



```
  SELECT ?occupation
  WHERE {
  	?person objectrole:hasRole ?occupation .
  	FILTER (?person = :alessandro_adamou)
  }

```

* + CQ2



```
  SELECT ?project
  WHERE {
  	?person :worksAt ?project .
  	FILTER (?person = :alessandro_adamou)
  }

```

* + CQ3



```
  SELECT ?funder
  WHERE {
  	?project :isFundedBy ?funder .
  	FILTER (?project = :iks)
  }

```

* + CQ4



```
  SELECT ?topic
  WHERE {
  	?project :hasTopic ?topic .
  	FILTER (?project = :iks)
  }

```

* ontology URI:


##   Story 6


* Priority: high
* Title: co-authoring of research products
* Description:



```
  Aldo Gangemi and Alessandro Adamou have written a conference paper on “Kali-ma”, 
  an application for interaction customization. It has been published at the ISWC 2011 conference.   

```

* Status:
* Assigned to Pair: Luca Iori e Gioele Barabucci
* Competency questions:
	1. Who wrote a certain paper?
	2. What is the topic of a certain paper?
	3. How many papers have been published in a certain conference?
	4. When has a certain paper been published?
	5. In which conference was a paper presented?
	6. When was a certain conference held?
* SPARQL queries:
	+ CQ 1:



```
  SELECT ?author 
  WHERE {
     ?author authoring:isAuthorOf ?paper .
     FILTER (?paper = :kali_ma)
  }

```

* + CQ 2:



```
  SELECT ?topic
  WHERE {
      ?paper papertopic:hasTopic ?topic .
      FILTER (?paper = :kali_ma)
  }

```

* + CQ 3:



```
  SELECT ?article
  WHERE {
      ?conf_setting timeindexedsituation:forEntity ?conference .
      ?conf_setting conference:hasPaper ?article .
      FILTER (?conference = :iswc_2011)
  }

```

* + CQ 4:



```
  SELECT ?article_time
  WHERE {
      ?conf_setting timeindexedsituation:forEntity ?conference .
      ?conf_setting conference:hasPaper ?article .
      ?conf_setting timeindexedsituation:atTime ?article_time .
      FILTER (?article = :kali_ma)
  }

```

* + CQ 5:



```
  SELECT ?conference
  WHERE {
      ?conf_setting timeindexedsituation:forEntity ?conference .
      ?conf_setting conference:hasPaper ?article .
      FILTER (?article = :kali_ma)
  }

```

* + CQ 6:



```
  SELECT ?time
  WHERE {
      ?conf_setting timeindexedsituation:forEntity ?conference .
      ?conf_setting timeindexedsituation:atTime ?time .
      FILTER (?conference = :iswc_2011)
  }

```

* ontology URI:



```
  [http://ontologydesignpatterns.org/cpont/cnr/story6.owl](http://ontologydesignpatterns.org/cpont/cnr/story6.owl "http://ontologydesignpatterns.org/cpont/cnr/story6.owl")

```

##   Story 7


* Priority: low
* Title: location of institutes
* Description:



```
  The ISTC (Institute for cognitive science and technology) has several offices located in different places. 
  The headquarter is located in Rome, in via San Martino della Battaglia 44. There are other offices in Rome, and one in Padova.  

```

* Status: delivered
* Assigned to Pair: Marcello Ceci & Lino Possamai
* Competency questions:



```
1) Which offices does a certain organization have?
2) How many offices does a certain organization have?
3) where is the HQ of a certain organization located?
4) Where are the offices of a certain organization located?

```

* SPARQL queries:


CQ1:




```
SELECT ?offices
WHERE {:istc_institute  :hasOffice ?offices.}

```

CQ2:




```
SELECT Count(?offices)
WHERE { :istc_institute  :hasOffice ?offices.}

```

CQ3:




```
SELECT ?address ?city
WHERE { :istc_institute  :hasHQ ?hq.
 ?hq place:hasLocation ?address.
 ?address place:hasLocation ?city}

```

CQ4:




```
SELECT DISTINCT ?offices ?address ?location
WHERE {
 {   :istc_institute  :hasOffice ?offices .
 ?offices place:hasLocation ?location .
 } UNION {
   :istc_institute  :hasOffice ?offices .
 ?offices place:hasLocation ?location .
 ?offices place:hasAddress ?address . }}

```

* ontology URI:


[http://ontologydesignpatterns.org/cpont/cnr/locationOfInstitutes.owl](http://ontologydesignpatterns.org/cpont/cnr/locationOfInstitutes.owl "http://ontologydesignpatterns.org/cpont/cnr/locationOfInstitutes.owl")



##   Story 8


* Priority: high
* Title: research interests and responsibilities
* Description:



```
  Aldo Gangemi belongs to the ISTC. His research topics are: ontology design, semantic web, and lexical semantics. 
  He is responsible for the “Semantic Intraweb” thematic project whose topic is semantic search and semantic technologies.   

```

* Status: delivered
* Assigned to Pair: Basile, Bragaglia
* Competency questions:



```
1) Which organization a person belongs to?
2) Who are the members of a certain organization?
3) What are the research topics of a certain member?
4) Who works on a certain research topic?
5) Who is responsible for a certain project?
6) What projects is a person responsible for?
7) What is the name of a certain project?
8) What are the topics of a certain project?
9) What projects belong to a certain topic?

```

* Contextual statements:



```
A thematic project must have at least one responsible

```

* SPARQL queries:



```
1) Which organization a person belongs to?
   SELECT ?organization
   WHERE {
       :aldo_gangemi membership:isMemberOf ?organization.
   }
2) Who are the members of a certain organization?
   SELECT ?member
   WHERE {
       membership:istc membership:hasMember ?member .
   }
3) What are the research topics of a certain member?
   SELECT ?topic
   WHERE {
       :aldo_gangemi topics:hasTopic ?topic .
   }
4) Who works on a certain research topic?
   SELECT ?member
   WHERE {
       topics:ontology_design topics:isTopicOf ?member .
       ?member rdf:type :Member .
   }
5) Who is responsible for a certain project?
   SELECT ?member
   WHERE {
       ?member :isResponsibleFor :semantic_intraweb .
   }
6) What projects is a person responsible for?
   SELECT ?project
   WHERE {
       ?project :hasResponsible :aldo_gangemi .
   }
7) What is the name of a certain project?
   SELECT ?name
   WHERE {
        :semantic_intraweb :hasProjectName ?name .
   }
8) What are the topics of a certain project?
   SELECT ?topic
   WHERE {
       :semantic_intraweb topics:hasTopic ?topic .
   }
9) What projects belong to a certain topic?
   SELECT ?project
   WHERE {
       topics:semantic_search topics:isTopicOf ?project .
       ?project rdf:type :Project .
   }

```

  




* ontology URI: [http://ontologydesignpatterns.org/cpont/cnr/interests\_responsibilities.owl](http://ontologydesignpatterns.org/cpont/cnr/interests_responsibilities.owl "http://ontologydesignpatterns.org/cpont/cnr/interests_responsibilities.owl")


##   Story 9


* Priority: medium
* Title: management roles
* Description:



```
  Francesco Beltrame is the director of the “ICT (Information and Communication Technology)” department, 
  and Cristiano Castelfranchi is the director of the “ISTC (Institute for cognitive science and technology)”

```

* Status: Delivered
* Assigned to Pair: Marcello Ceci & Possamai Lino
* Competency questions:



```
1) Who is the director of a certain organization?
2) What is the role played by a certain person in a certain organization

```

* SPARQL queries:


  





```
SELECT ?solution
WHERE {
    :ICT_department :hasDirectiveInstitution ?obj .
?obj :isDirectiveRoleOf ?solution .
}
SELECT ?obj
WHERE {
    :ICT_department :hasDirectiveInstitution ?obj .
:francesco_beltrame :hasDirectorRole ?obj.
}

```

  




* ontology URI:


[http://ontologydesignpatterns.org/cpont/cnr/story9.owl](http://ontologydesignpatterns.org/cpont/cnr/story9.owl "http://ontologydesignpatterns.org/cpont/cnr/story9.owl")



##   Story 10


* Priority: medium
* Title: thematic projects’ characteristics
* Description: Thematic projects' characteristics



```
  the “Semantic Intraweb” thematic project is supported by the ICT department and executed by the ISTC. 
  It is currently active, and has two work packages. Its responsible person is Aldo Gangemi. 
  Its first year of activity is 2006 and its expected ending yearis 2012. 

```

* Status: delivered
* Assigned to Pair: Basile, Bragaglia
* Competency questions:



```
1) What projects are supported by a certain department?
2) What department supports a certain project?
3) What projects are executed by a certain institute?
4) What institute executes a certain project?
5) What is the status of a certain project in a certain moment?
6) How many working packages does a project have?
7) Who is responsible for a certain project?
8) What projects is a person responsible for?
9) When did a certain project start?
10) When is a certain project expected to end?

```

* SPARQL queries:



```
1) What projects are supported by a certain department?
   SELECT ?project
   WHERE {
       ?project :isSupportedBy :ict .
   }
2) What department supports a certain project?
   SELECT ?department
   WHERE {
       ?department :supports :semantic_intraweb .
   }
3) What projects are executed by a certain institute?
   SELECT ?project
   WHERE {
       ?project :isExecutedBy :istc .
   }
4) What institute executes a certain project?
   SELECT ?institute
   WHERE {
     ?institute :executes :semantic_intraweb .
   }
5) What is the status of a certain project in a certain moment?
   SELECT ?status
   WHERE {
       :semantic_intraweb projectstatus:isProjectOf ?projectstatus .
       :semantic_intraweb_activity projectstatus:isActivityIntervalOf ?projectstatus .
       ?projectstatus projectstatus:hasStatus ?status .
   }
6) How many working packages does a project have?
   SELECT ?workingpackages
   WHERE {
       :semantic_intraweb :hasPackages ?workingpackages .
   }
7) Who is responsible for a certain project?
   SELECT ?person
   WHERE {
       ?person :isResponsibleFor :semantic_intraweb .
   }
8) What projects is a person responsible for?
   SELECT ?project
   WHERE {
       ?project :hasResponsible :aldo_gangemi .
   }
9) When did a certain project start?
   SELECT ?date
   WHERE {
       ?projectstatus projectstatus:hasProject :semantic_intraweb .
       ?projectstatus projectstatus:hasStatus :active .
       ?projectstatus projectstatus:hasActivityInterval ?activity .
       ?activity activityinterval:hasStart ?date .
   }
10) When is a certain project expected to end?
   SELECT ?date
   WHERE {
       ?projectstatus projectstatus:hasProject :semantic_intraweb .
       ?projectstatus projectstatus:hasStatus :active .
       ?projectstatus projectstatus:hasActivityInterval ?activity .
       ?activity activityinterval:hasEnd ?date .
   }

```

* ontology URI:
* notes: talking with the customer, it emerged that he may want to know the status of a certain project over time


##   Story 11


* Priority: medium
* Title: conferences
* Description:



```
  The EKAW 2008 conference was chaired by Aldo Gangemi who, as such, is also the editor of the conference proceedings. 
  It is one of a series of conferences on Knowledge Engineering and Knowledge Management that is held biennially. 
  Aldo Gangemi also chaired SWAP 2008, which was held in Rome in December.

```

* Status:Delivered
* [http://ontologydesignpatterns.org/cpont/cur/story11.owl](http://ontologydesignpatterns.org/cpont/cur/story11.owl "http://ontologydesignpatterns.org/cpont/cur/story11.owl")
* Assigned to Pair:


Distefano Zuppiroli



* Competency questions:


1)When an event is done?
2)where an event is done?
3)what event is taking place?
4)Who is the editor in an event?
5)who is the chair in an event?
6)how often an event takes place?
7)What is the genre of conference?



* SPARQL queries:


1) SELECT ?Event




```
 WHERE {
 	?Event :whenEventTakePlace ?DataEvent .
 }

```

2) SELECT ?Event




```
 WHERE {
 	?Event location:isLocationOf ?City .
 }

```

3) SELECT ?Topic




```
 WHERE {
 	?Topic :isTopic ?Event .
 }

```

4) SELECT ?Person




```
 WHERE {
 	?Event :editedBy ?Person .
 }

```

5)




```
 SELECT ?Person
 WHERE {
 	?Person :isChair ?Event .
 }

```

6) SELECT ?Event




```
 WHERE {
 	?event :frequencyOfHeld ?Event .
 }

```

7) SELECT ?conference




```
 WHERE {
 	?topic :hasTopic ?conference.
 }

```

* ontology URI:


##   Story 12


* Priority: medium
* Title: conference proceedings and publications
* Description:



```
  EKAW 2008 conference proceedings include 23 research papers and 12 short papers. 
  SWAP workshop proceedings include a paper entitled “SAscha: A RIA Approach for 
  Supporting Semantic Web Services in the Italian Interoperability Framework”, 
  written by Alessandro Adamou on semantic web services.

```

* Status: DELIVERED
* Assigned to Pair: Andrea Burattin and Antonio Lieto
* Competency questions:


1. Which is the name of a conference?
2. Does a conference have proceedings?
3. How many research papers and short papers a proceedings contains?
4. In which proceedings a certain paper is contained?
5. Who are the authors of a certain paper?
6. Which are the topics of a paper?


* SPARQL queries:
	+ CQ1



```
  SELECT ?name
  WHERE {
  	?conference :hasTitle ?name .
  	FILTER (?conference = :ekav_2008)
  }

```

* + CQ2



```
  SELECT ?proceedings
  WHERE {
  	?conference :hasEvents ?event .
  	?event conferenceevents:hasProceedings ?proceedings .
  	FILTER (?conference = :ekav_2008)
  }

```

* + CQ3



```
  SELECT ?countPaper ?countShortPaper
  WHERE {
  	?proceedings proceedings:papersIncluded ?countPaper .
  	?proceedings proceedings:shortPapersIncluded ?countShortPaper .
  	FILTER (?proceedings = proceedings:ekaw_2008_proceedings)
  }

```

* + CQ4



```
  SELECT ?proceedings
  WHERE {
  	?proceedings proceedings:proceedingsContainsPaper ?paper .
  	FILTER (?paper = proceedings:sascha_a_ria_approach_for_supporting_semantic_web_services_in_the_italian_interoperability_framework)
  }

```

* + CQ5



```
  SELECT ?authors
  WHERE {
  	?paper proceedings:hasAuthor ?authors .
  	FILTER (?paper = proceedings:sascha_a_ria_approach_for_supporting_semantic_web_services_in_the_italian_interoperability_framework)
  }

```

* + CQ6



```
  SELECT ?topics
  WHERE {
  	?paper proceedings:hasTopic ?topics .
  	FILTER (?paper = proceedings:sascha_a_ria_approach_for_supporting_semantic_web_services_in_the_italian_interoperability_framework)
  }

```

* ontology URI:


We have used the following Ontology design pattern: partecipation and collection entities.



##   Story 13


* Priority: high
* Title: finding experts in related topics
* Description:



```
  Giovanni Adamo is a researcher at CNR and he is looking for other CNR researchers to create a team for a project on semantic
  technologies. He wants to find researchers interested in all topics related to semantic technologies: semantic wikis, 
  semantic web, ontology design, etc.

```

* Status:
* Assigned to Pair: Luca Iori and Gioele Barabucci
* Competency questions:
	1. Who works in a certain research institution?
	2. In which research topics is a certain researcher interested in?
	3. Which research topics are related to a certain other research topic?
	4. Which researchers of a certain research institution are interested in a certain research topic?
* SPARQL queries:
	+ CQ 1:



```
  SELECT ?person
  WHERE {
      ?person researchinstitute:isResearcherOf ?institution .
      FILTER (?institution = :cnr)
  }

```

* + CQ 2:



```
  SELECT ?topic
  WHERE {
      ?person :isInterestedIn ?topic .
      FILTER (?person = :learco_ferrari)
  }

```

* + CQ 3:



```
  SELECT ?topic
  WHERE {
      { ?base_topic topic:nearTopicTo ?topic . }
      UNION { ?base_topic topic:isSubTopicOf ?topic . }
      UNION { ?base_topic topic:hasSubTopic ?topic . }
      UNION { ?base_topic topic:overlappingTopic ?topic . }
      FILTER (?base_topic = researchtopic:semantic_technologies)
  }

```

* + CQ 4:



```
  SELECT ?researcher
  WHERE {
      ?researcher researchinstitute:isResearcherOf ?institution .
      ?researcher :isInterestedIn ?topic .
      FILTER (?topic = researchtopic:semantic_web)
      FILTER (?institution = :cnr)
  }

```

* ontology URI:



```
  [http://ontologydesignpatterns.org/cpont/cnr/story13.owl](http://ontologydesignpatterns.org/cpont/cnr/story13.owl "http://ontologydesignpatterns.org/cpont/cnr/story13.owl")

```

##   Story 14


* Priority: medium
* Title: project meetings
* Description:



```
  Project meetings are events that are held in one particular location during one or several days. 
  Between November 11-13 2009 a meeting of the EU-funded IKS project was held in Rome, at the head office of the ISTC 
  (Institute for cognitive science and technology), in San Martino della Battaglia 44. Participants of the meeting where  
  Aldo Gangemi, Valentina Presutti and Eva Blomqvist, all belonging to ISTC, and also other people from other institutions.

```

* Status: Delivered
* Assigned to Pair:


Distefano Zuppiroli



* Competency questions:


1)where the meetings are held?
2)when meetings take place?
3)How long the meeting
4)Who participates in the meeting?
5)institution to which the parties belong to the meeting?



* SPARQL queries:


1)SELECT ?City




```
  WHERE {
      ?Institute location:hasLocation ?City .
} 

```

2)SELECT ?TimeInterval




```
  WHERE {
      ?Event :whenEventTakePlace ?TimeInterval.
}

```

3)SELECT ?Event




```
WHERE {
	?event :howLongTheMeeting ?Event   .
} 
4)SELECT ?Person
WHERE {
	?Event :eventPartecipation ?Person   .
} 

```

5) SELECT ?Institute




```
WHERE {
	?Institute :institutePovenience ?Person   .
} 

```

* ontology URI:[http://ontologydesignpatterns.org/cpout/cur/story14.owl](http://ontologydesignpatterns.org/cpout/cur/story14.owl "http://ontologydesignpatterns.org/cpout/cur/story14.owl")


##   Story 15


* Priority: low
* Title: conference participation
* Description:



```
  Aldo Gangemi participated in the ISWC 2009 conference, but he didn't present any paper there. However, in ESWC 2009 Aldo presented a paper entitled "Frame Detection over the Semantic Web" that he co-authored with Alfio Gliozzo and Valentina Presutti who are also researchers of the ISTC (Institute for cognitive science and technology). Additional co-authors of the paper were Bonaventura Coppola and Davide Picca who are affiliated to other organizations.

```

* Status:delivered
* Assigned to Pair:Distefano Zuppiroli
* Competency questions:


1)To which a person participates in conference?
2)What are the titles of papers presented at conferences?
3)What is the author of each article?
4)What is the co-author of each article?
5)Researchers in which institutions perform research?



* SPARQL queries:


1) SELECT ?Conference
WHERE {




```
   ?Person situation:hasSetting ?Conference .

```

}


2) SELECT ?Paper
WHERE {




```
   ?Paper :paperPresentedIn ?Conference .

```

}



* ontology URI:[http://ontologydesignpatterns.org/cpout/cur/story15.owl](http://ontologydesignpatterns.org/cpout/cur/story15.owl "http://ontologydesignpatterns.org/cpout/cur/story15.owl")


#   Integration


##   Integrated modules and versioning


Physical URIs of newly published modules that integrate the single stories are listed here.


The last modified version of the integrnation module is always 


[http://ontologydesignpatterns.org/cpont/cnr/cnr.owl](http://ontologydesignpatterns.org/cpont/cnr/cnr.owl "http://ontologydesignpatterns.org/cpont/cnr/cnr.owl")


Old versions of any module are available with the following URI pattern


[http://ontologydesignpatterns.org/cpont/cnr/old](http://ontologydesignpatterns.org/cpont/cnr/old "http://ontologydesignpatterns.org/cpont/cnr/old")<version\_number>/<filename>.owl
Current


Old versions:



* Original ontologies from stories: [http://ontologydesignpatterns.org/cpont/cnr/old1](http://ontologydesignpatterns.org/cpont/cnr/old1 "http://ontologydesignpatterns.org/cpont/cnr/old1")
* Integration of the stories 3, 6 and 8: [http://ontologydesignpatterns.org/cpont/cnr/old2](http://ontologydesignpatterns.org/cpont/cnr/old2 "http://ontologydesignpatterns.org/cpont/cnr/old2")
* Integration of the story 4: [http://ontologydesignpatterns.org/cpont/cnr/old3](http://ontologydesignpatterns.org/cpont/cnr/old3 "http://ontologydesignpatterns.org/cpont/cnr/old3")


##   Guidelines and feedback


Here goes the entire feedback from the integrating group to other developers.



##   Testing


* Syntax Checking for imports and namespaces
* Check provided modules for consistency
* Retrieve potential matches
* Check potential inconsistencies


###   Alignment notes


* Story 3 - Story 6 - Story 8
	+ researchProducts:isTopicOf (story 3) is a subproperty of topic:isTopicOf (of Topic pattern)
	+ researchProducts:isTopicOf (story 3) is an equivalent property of topics:isTopicOf (story 8)
	+ paperTopic:isTopicOf (story 6) is a subproperties of researchProducts:isTopicOf (story 3)
	+ topics:Topic (story 8) is equivalent to researchProducts:Topic (story 3) are equivalent classes and subclasses of topic:Topic (of Topic pattern)
	+ topic:Concept (Topic pattern) is equivalent to classification:Concept (Classification pattern)
	+ conference:Conference (story 6) is a subclass of partecipation:Event (Partecipation pattern)
	+ authoring:Paper (story 6) is a subclass of resarchProduct:Publication (story 3)
	+ REMOVED the subclass axiom between authoring:Paper (story 6) and partecipation:Event (Partecipation pattern)
	+ Consistency checked and queried!!!


* Story 4
	+ membership:Organization (story 8) is equivalent to organization:Organization (story 4)
	+ a researchproducts:Researcher (story 3) is equivalent to personjob:hasJob some personjob:Researcher (story 4)
	+ added RDFS annotation to personjob:Researcher (story 4)
	+ researchprodcts:Person (story 3) is equivalent to personjob:Person (story 4)
	+ update (story 6): conference:ConferenceSituation is subclass of situation:isSettingFor (Situation pattern) some conference:Conference (story 6)
	+ Consistency checked and queried!!!


* Story 11
	+ roleinconference:Person (story 11) is equivalent to personjob:Person (story 4)
	+ story11:Topic (story 11) is equivalent to topic:Topic (Topic pattern)
	+ story11:Conference (story 11) is equivalente to conference:Conference (story 6)
	+ event:Event (story 11) is subclass of partecipation:Evente (Partecipation pattern)


###   Post-integration queries


Regression testing on the providers' original SPARQL queries, and its results, are published here.



###   Reasoning / Unit tests


Here the modules are checked for consistency and unit tests for restrictions, disjointness axioms etc. are performed.





Retrieved from "[http://ontologydesignpatterns.org/wiki/Training:PhD\_Course\_on\_Computational\_Ontologies\_%40\_University\_of\_Bologna/Collaborative\_modeling\_with\_XD](../../Training/PhD_Course_on_Computational_Ontologies_@_University_of_Bologna/Collaborative_modeling_with_XD.md)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [Exercise](../../Category/Exercise.md "Category:Exercise")