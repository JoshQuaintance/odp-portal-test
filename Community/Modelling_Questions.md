#  Modelling Questions


__Title:__ Modeling Questions


__Description:__ This problem came up in the context of the [W3C Decision Incubator activity](http://www.w3.org/2005/Incubator/decision/wiki/Main_Page "http://www.w3.org/2005/Incubator/decision/wiki/Main_Page"), however, it is more general than the decision-making domain. It is about how to formally represent questions in OWL. 


For instance, if I ask a question like "Where did this emergency occur?" I could simply represent it as a string. However, the question contains a lot of information, so in some cases one might want to represent it formally, and possibly reason on the question itself. For instance, we may want to derive that the answer should be of type "location" from the fact that the question uses the keyword "where".


We have identified two main aspects of this modeling issue:



1. How can we refer to the detailed description of the question?
2. How can we model the semantics of the question itself?


The first issue concerns the case when we would like to include both the question as a string, i.e., the human readable version of the question, and the question as a formal model. In this case we may have a class "Question", with a string property containing its representation in natural language. How do we now link also a formal description of this question, i.e., a set of triples, to the question class?


The second issue concerns how to represent the semantics of the question itself, i.e., an ontology for modeling those triples we wanted to refer to above. We would like to model things such as, the variable of the question, the expected answer type, any other constraints set in the question etc. For instance, in order to be able to ask questions such as: What is the expected answer type of this question? Is this answer correct with respect to the constraints of this question?


There exist some question classifications originating in expert systems and question answering, however, we are not aware of any OWL models. 


__Diagram__
_(this article has no graphical representation)_



#  About


  




#  Additional information


#  References


[Add a reference](index.php@title=Odp%253AAdd_reference&subject=Community%253AModelling+Questions.html "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_reference&subject=Community%3AModelling+Questions")


  




 [List of Modeling Issues](../Community/Main.md "Community:Main") | [Post a new modeling issue](../Community/PostModelingIssue.md "Community:PostModelingIssue") | [Add a comment in the discussion page](index.php@title=Odp%253AAdd_comment&target=Community_talk%253AModelling_Questions.html#New_comment "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_comment&target=Community_talk:Modelling_Questions#New_comment")


Retrieved from "[http://ontologydesignpatterns.org/wiki/Community:Modelling\_Questions](../Community/Modelling_Questions.md)"
 [Categories](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [ModelingIssue](../Category/ModelingIssue.md "Category:ModelingIssue") | [Submitted to event](../Category/Submitted_to_event.md "Category:Submitted to event")