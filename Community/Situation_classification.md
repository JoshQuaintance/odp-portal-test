#  Situation classification


__Title:__ Situation classification


__Description:__ Classical problem-solving in AI and knowledge engineering requires a full-fledged knowledge representation system, including languages for representing the domain and the axioms/rules that hold for it (the problem space), as well as algorithms to find a solution to that problem, if any. Classical approaches use different languages for the representation of the problem versus the representation of the solution, e.g. declarative vs. procedural.
However, there are many requirements in domain modelling which require to talk about both the problem and solution spaces within a same universe of discourse. This is the case of legal knowledge (factual knowledge and legal cases vs. normative knowledge), services, planning and control knowledge (actual facts vs. expected facts), diagnostic knowledge and situational awareness (e.g. bare facts vs. typically unwanted facts), etc. All those cases fit into the abstract task of "classifying a situation" according to possibly incomplete, alternative or loose constraints, where those constraints must be explicit and explicitly linked to the representation of a situation.
There are content patterns for representing situation classification, such as descriptionandsituation.owl, which relies on reification of conepts and relations. These patterns can represent situations and descriptions, and their given links (e.g. entities of a situation that play roles from a description, values of a situation that fit parameters from a description, etc.). 
But it's very hard to represent in general (not based on locally defined axioms, e.g. owl:equivalentClass axioms for a particular situation/description pair) how to:


1) make a situation emerge out of scattered facts
2) decide if a situation (or a set of facts) can be (partly or fully) classified under a description
3) evaluate which description fits best a certain set of facts
etc.


Classical approaches represent situation classification within some algorithm or in the semantics of some appropriate meta-model. The modeling issue here is: 


---) can we approximate generalized representations, for at least some situation classification tasks, by using OWL2 (e.g. with features such as punning, property chains, reflexivity) and regular description logic reasoners. In other words, is it possible to represent situation classification so that it reduces to a concept classification problem? 


__Diagram__
_(this article has no graphical representation)_



#  About


  




#  Additional information


#  References


[Add a reference](index.php@title=Odp%253AAdd_reference&subject=Community%253ASituation+classification.html "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_reference&subject=Community%3ASituation+classification")


  




 [List of Modeling Issues](../Community/Main.md "Community:Main") | [Post a new modeling issue](../Community/PostModelingIssue.md "Community:PostModelingIssue") | [Add a comment in the discussion page](index.php@title=Odp%253AAdd_comment&target=Community_talk%253ASituation_classification.html#New_comment "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_comment&target=Community_talk:Situation_classification#New_comment")


Retrieved from "[http://ontologydesignpatterns.org/wiki/Community:Situation\_classification](../Community/Situation_classification.md)"
 [Categories](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [ModelingIssue](../Category/ModelingIssue.md "Category:ModelingIssue") | [Submitted to event](../Category/Submitted_to_event.md "Category:Submitted to event")