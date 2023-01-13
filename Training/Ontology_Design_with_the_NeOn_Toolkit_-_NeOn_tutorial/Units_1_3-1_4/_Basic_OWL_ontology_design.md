__Problem__:
[Opening NTK, creating a project, creating a new ontology (Michael)]


[Natural language and formal interpretation]


Formal interpretation is not (only:)) an academic game
It gives us a precise way to establish what we are talking about, and therefore to provide reliable automated inferences when needed.


Natural language is able to describe very different types of facts with the same structure, for example:



* Ahab hates Moby Dick [fact]
* Captain Ahab is in command of the Pequod [fact]
* Moby Dick is white [attributive fact]
* The Pequod is a whaler [classification fact]
* A whaler is a whaling ship [meaning fact]
* Whaler is six characters long [informational fact]
* Whaler is a class [formal fact]
* Whales are a delicious food for Japanese people [contextual fact]
* Moby Dick represents the internal fighting of Ahab's [interpretive fact]


But this functionality of natural language cannot be reproduced easily for machine interpretation. The formal interpretation of OWL can help us with that.


Each entity in an ontology is a web resource, and has a URI.
Each fact can be expressed as a triple.


[RDF exercise]


basic structure: Subject-Predicate-Object


---> Let's create a new ontology "Moby Dick"



* Ahab hates Moby Dick
* Moby Dick is a whale


If the fact includes three entities, you can embed a triple in another



* { Whales are a delicious food } for Japanese people


But this is not allowed in OWL. During the training we will see how to represent also such cases.
As a matter of fact, you can declare any fact in RDF, even "unusual" or "abnormal" ones:



* Moby Dick is white
* Moby Dick is black
* Moby Dick is in command of the Pequod
* Ahab hates the third character of the white whale
* Ahab is a class


In order to limit (and to guide) the design of ontologies, OWL restricts the expressivity of RDF.
No more is any triple allowed, but only those that respect the constraints of OWL formal semantics


[OWL exercises: 1) types, subclasses, and inheritance]



* Ahab hates Moby Dick
* Ahab is a human
* Moby Dick is a whale
* Whale is a class
* Whale is a subclass of Mammal
* Whale is a subclass of AquaticOrganism
* Mammal is a subclass of Vertebrate
* Vertebrate is a group


Notice that some inferences are now allowed:



* Since Moby Dick is a whale, and whales are mammals, Moby Dick is a mammal
* Since Whale is a subclass of Mammal, and Mammal is a subclass of Vertebrate, then Whale is a subclass of Vertebrate


This is called inheritance.
But, if modelled as in the previous exercises, the following is prevented in OWL:


!\* Since Moby Dick a whale, and Whale is a class, then Moby Dick is a class
!\* Since Mammal is a subclass of Vertebrate, and Vertebrate is a group, then Mammal is a group


Lesson learnt: in OWL we must distinguish when "is a" means "type", and when it means "subclass"
Tomorrow we'll see more on how to represent these cases.


  

\\\\\changed from here on\\\\\
[OWL exercises: 2) disjointness and consistency: use Radon to check the ontology after each addition]



* Whales are not humans


In formal semantic languages, we can usually state when two classes are disjoint.
This provides greater clarity, and works fine for "integrity checks", called "coherency" or "consistency", in ontologies
Equipped with the disjointWith axiom, we can now exclude the following:


!\* Moby Dick is a human
!\* Ahab is a Whale


since they would lead the ontology to an "inconsistency"


and we can also exclude the following:


!\* Whamans are whales and humans


since they would lead the ontology to an "incoherence"


  

[OWL exercises: 3) domains, ranges, inverses, subproperties, materialization, and classification]



* Whales can be food for Japanese humans
* Being able to be food for something implies being able to be fed by something
* Moby Dick can be food for Yukio
* Hating something implies disliking it


Some new inferences are now allowed:



* Since Moby Dick can be food for Yukio, then Yukio can be fed by Moby Dick
* Since Ahab hates Moby Dick, he dislikes it


This is called materialization.



* Since Yukio can be fed by Moby Dick, and (as far as we know) only Japanese humans can be fed by whales, then Yukio is a Japanese human


This is called classification.
But the following is prevented: (open source, disjointness etc.)


!\* Yukio can be food for Moby Dick


Since the Web is an open world, if we say something that is not explicitly put in our axioms, we cannot exclude it, and then we have to add a new axiom, e.g.:


!\* Since Yukio can be food for Moby Dick, which is a whale, and whales can be food for Japanese humans, then Yukio is also a whale, while Moby Dick is also a Japanese human


But this generates an inconsistency, if we had modelled JapaneseHuman as a subclass of Human, since Human and Whale are disjoint classes, and JapaneseHuman is also disjoint with Whale, for ->inheritance


  

[OWL exercises: 4) sameness and difference]


Due to open world assumption, it is important to explicitly declare if any two individuals are the same or are different (when this is known).



* Moby Dick is the same as "The White Whale"
* Ahab is different from Yukio


  

The formal semantics of OWL is currently based mostly on so called "description logics". The main difference that description logics have introduced is the generalization of classes to kinds of construct that can be interpreted as a set of individuals.


---> Let's create a new ontology "Aquatic organisms"


  

[OWL exercises: 5) boolean concepts]


Firstly, "boolean" class constructors:



* The class of things that are mammals and aquatic organisms
* The class including aquatic mammals, fishes and crustaceans
* The class of things that are not fishes


  

[OWL exercises: 6) restrictions]


Secondly, "relational" class constructors:



* The class of things that only live in a marine habitat
* The class of things that live in at least one marine habitat
* The class of things that only live in demersal habitat
* The class of things that only live in either benthic or pelagic habitat
* The class of things that have taxonomic species "Monodon monoceros"


  

[OWL exercises: 7) nominals]


Thirdly, "enumerating" class constructors:



* The class of the following things: demersal, benthic, and pelagic


  

[OWL exercises: 8) equivalence and automated subsumption/classification] 


Differently from other conceptual modelling languages, OWL allows to state formal equivalence between two classes. 
Equivalence works implictly with class constructors (ontology APIs generate internal classes that are equivalent to class constructors), but equivalence can be stated explictly.


---> Let's create a new ontology "Cetaceans"



* Aquatic mammals are mammals and aquatic organisms
* Aquatic organisms only include aquatic mammals, fishes and crustaceans
* Whales are not fishes
* Demersal fishes are fishes that live in demersal habitat
* Benthopelagic fishes are fishes that only live either in benthic or pelagic habitats
* Narwhals are whales that have taxonomic species "Monodon monoceros"
* The marine habitats are: demersal, benthic, and pelagic


  

[OWL exercises: 9) symmetry and transitivity]


Object properties can be symmetric, or transitive. "Sibling" is an example of both symmetric and transitive object property.



* siblingOrder is symmetric
* siblingOrder is transitive
* Cetacea and Artyodactyla (classifying even-toed ungulates) are sibling orders of superorder Laurasiatheria
* Within Cetacea, Monodon monoceros is a sibling species of Orcynus Orca, which is a sibling species of Balaenoptera musculus (blue whale)


  

[OWL exercises: 10) imports]



* Everything that is true of Cetaceans ontology is true for Moby Dick ontology



__Solutions__:





Retrieved from "[http://ontologydesignpatterns.org/wiki/Training:Ontology\_Design\_with\_the\_NeOn\_Toolkit\_-\_NeOn\_tutorial/Units\_1\_3-1\_4:\_Basic\_OWL\_ontology\_design](../../../Training/Ontology_Design_with_the_NeOn_Toolkit_-_NeOn_tutorial/Units_1_3-1_4/_Basic_OWL_ontology_design.md)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [Exercise](../../../Category/Exercise.md "Category:Exercise")