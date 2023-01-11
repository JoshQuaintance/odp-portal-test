##   --[MichaelUschold](../User/MichaelUschold.md "User:MichaelUschold") 20:05, 26 February 2010 (UTC)


Can you give a bit more detail here?



* Give some examples of _abstraction criteria_
* Why do you need multiple abstractions at the same time?
* Can you express your needs as one or more competency questions?


##   --[BenedictoRodriguezCastro](../User/BenedictoRodriguezCastro.md "User:BenedictoRodriguezCastro") 17:45, 3 March 2010 (UTC)


__Note:__ 
This is still work in progress but I will try to characterize better the modeling problem that I am putting forward.



###   Give some examples of abstraction criteria


By "abstraction criteria" I actually intended to mean "alternative criteria to classify the abstractions of a domain concept" or also in other words when there are "competing classification criteria" available to model the representation of a domain concept.


This modeling problem is discussed in object-oriented design as the motivation to introduce "View Inheritance" [1]. "View Inheritance" corresponds to one of the 12 valid uses of inheritance identified by the author (see page 824 of [1]).


As an example from the object-oriented design, consider the alternative criteria that are avaible to classify the abstraction of a simple domain concepts such as "employee" (page 852 in [1]):



* Employee: by contract type (permanent vs. temporary), by job type (engineering, administrative, managerial).


But similar examples exist in the ontology design field such us "wine"[2] and "pizza"[3]:



* Wine: color, region, flavour, ocassion, etc.
* Pizza: base (deep pan, thin), topping (cheese, meat, vegetable, etc.), name (margherita, american, etc.)


###   Why do you need multiple abstractions at the same time?


Because there are cases when the application intended to use the ontology requires the multiple abstractions available of the domain concept to be represented in the ontology.


For example, let us think of a web site that attemtps to provide wine recommendations to its visitors or a web site to order pizza.



###   Can you express your needs as one or more competency questions?


I think from the examples given, it is somewhat intuitive to identify competency questions that would suggest to the ontology engineer to capture the multiple abstractions available to represent the domain concept in question.


For example, in the case of "wine":



* Allow me to select a bottle of wine by color, region, flavour and(or) ocassion.


In the case of "pizza":



* Allow me to select a pizza based on the type of base, the toppings and(or) the name.


###   Additional Comments


After some time looking at this type of modeling problem, another line of research that opened up is the notion of "facet analisys" and "faceted classification" in Library Science.


It seems that there is a strong correlation across different disciplines regarding how they address the modeling problem presented here:



* "View Inheritance" in Object-Oriented Design (see page 824 of [1]).
* The "polyhierarchies" or "semantic axes" refered to in the "Normalization Ontology Design Pattern" in Ontology Design[4][5].
* "Facet Analysis" and "Facetted Classification" in Library Science. See example on how to model the concept of "dish detergent" in [6].


###   References


[1] Bertrand Meyer. Object-Oriented Software Construction (Book/CD-ROM) (2nd Edition). Prentice Hall PTR, March 2000. [ISBN 0136291554](http://ontologydesignpatterns.org/wiki/Special:BookSources/0136291554).


[2] N. F. Noy and D. McGuinness. Ontology development 101: A guide to creating your first ontology. Technical Report SMI-2001-0880, Stanford Medical Informatics, Stanford, 2001. [http://www-ksl.stanford.edu/people/dlm/papers/ontology101/ontology101-noy-mcguinness.html](http://www-ksl.stanford.edu/people/dlm/papers/ontology101/ontology101-noy-mcguinness.html "http://www-ksl.stanford.edu/people/dlm/papers/ontology101/ontology101-noy-mcguinness.html")


[3] Matthew Horridge, Nick Drummond, Simon Jupp, Georgina Moulton, Robert Stevens. A Practical Guide To Building OWL Ontologies Using Protege 4 and CO-ODE Tools Edition 1.2. Technical report, The University Of Manchester, March 2009. [http://owl.cs.manchester.ac.uk/tutorials/protegeowltutorial/resources/ProtegeOWLTutorialP4\_v1\_2.pdf](http://owl.cs.manchester.ac.uk/tutorials/protegeowltutorial/resources/ProtegeOWLTutorialP4_v1_2.pdf "http://owl.cs.manchester.ac.uk/tutorials/protegeowltutorial/resources/ProtegeOWLTutorialP4_v1_2.pdf")


[4] Alan L. Rector. Modularisation of domain ontologies implemented in description logics and related formalisms including owl. In K-CAP '03: Proceedings of the 2nd international conference on Knowledge capture, pages 121{128, New York, NY, USA, 2003. ACM. [ISBN 1-58113-583-1](http://ontologydesignpatterns.org/wiki/Special:BookSources/1581135831).


[5] Normalization Ontology Design Pattern. [http://www.gong.manchester.ac.uk/odp/html/Normalisation.html](http://www.gong.manchester.ac.uk/odp/html/Normalisation.html "http://www.gong.manchester.ac.uk/odp/html/Normalisation.html")


[6] Denton, William. How to Make a Faceted Classification and Put It On the Web. Nov 2003. [http://www.miskatonic.org/library/facet-web-howto.html](http://www.miskatonic.org/library/facet-web-howto.html "http://www.miskatonic.org/library/facet-web-howto.html")



##   --[MichaelUschold](../User/MichaelUschold.md "User:MichaelUschold") 05 March 2010


This is a response to the comment left by Bene Rodriguez-Castro in the discussion tab.


A description logic provides a very natural way to characterize concepts/classes by multiple criteria using the idea of a restriction. Furthermore, the classification hierarchy is generated automatically for you.


The elaboration you gave is a very good continuation of this issue. You may wish to move some of it into the main issue page.





Retrieved from "[http://ontologydesignpatterns.org/wiki/Community\_talk:View\_Inheritance](../Community_talk/View_Inheritance.md)"