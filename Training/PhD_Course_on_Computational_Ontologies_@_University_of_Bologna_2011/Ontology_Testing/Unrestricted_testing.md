##   Ontology Testing


Parts of the ontology requirements are usually expressed as competency questions (CQs), i.e. natural language questions that the ontology should be able to provide answers to. Assuming that your module attempts to solve the two CQs, CQ1 and CQ2, obviously then in the ontology module there needs to be the facilities, i.e. classes, properties, axioms etc., such that it is possible to retrieve instances and/or literals that constitute the answer to the CQs.


Although CQs express what information the ontology should be able to provide, they do not say how this information is produced, i.e. if it is input into the ontology explicitly as assertions or produced through some inference mechanism. Therefore an ontology can have additional requirements, describing some desired inferences that the ontology should support. For instance, in an ontology about people we may define the class "parent" and say that any person who has at least one child is a parent. If we are not expecting the information about being a parent or not to be explicitly entered into the ontology's knowledge base, we are instead expecting it to be derived from the presence of "hasChild" relations. This is a reasoning requirement that requires the ontology to include the appropriate axioms to make this inference. 


Although the ability to perform correct inferences, and provide the resulting information as a result of queries, allow us to see that the ontology actually realizes its requirements, another important characteristic of an ontology is to allow as few erroneous facts and/or inferences as possible. A high-quality ontology allows exactly the desired inferences and queries, while avoiding to produce irrelevant or erroneous side-effects.


  

__Task:__



1. Download [this ontology module](http://www.ontologydesignpatterns.org/ont/training/musicindustry.owl "http://www.ontologydesignpatterns.org/ont/training/musicindustry.owl"), and put it in your ontology editor. Be sure you have SPARQL and reasoning support.
2. Create a new wiki page on this portal, and link it from this page (add your page at the last bullet in the list below), use the name template as it is indicated by the first bullet.
3. Copy the  [exercise template](http://ontologydesignpatterns.org/wiki/Training:PhD_Course_on_Computational_Ontologies_%40_University_of_Bologna_2011/Ontology_Testing/ExerciseTemplate "Training:PhD Course on Computational Ontologies @ University of Bologna 2011/Ontology Testing/ExerciseTemplate") and paste it in your exercise wiki page.
4. While you are working, __document what you are doing__, e.g. how are you performing your task in practice, how long time does it take, and what errors are you able to find in the table contained in your wiki page. Feel free to note down any additional comments you find relevant.
5. Try to plan your time, so that you try out different methods, i.e. don't spend all your time on one method. Approximately you should devote 2 hours to the exercise, so try to to have time for some different ideas.
6. When you feel satisfied with the testing, or when there is only 30 minutes left of the session (the tutor will warn you), please save the wiki page and [fill this questionnaire](http://stlab.istc.cnr.it/documents/PhDCourse/Bologna2011/TestingExerciseQuestionnaire2.txt "http://stlab.istc.cnr.it/documents/PhDCourse/Bologna2011/TestingExerciseQuestionnaire2.txt").
7. Send the questionnaire to _evabl444 -at- gmail -dot- com_ and _valentina -dot- presutti -at- cnr -dot-it_
8. Finalize your exercise on the wiki by May 30th.


* [Ornela Dardha](http://ontologydesignpatterns.org/wiki/Training:PhD_Course_on_Computational_Ontologies_%40_University_of_Bologna_2011/Ontology_Testing/OrnelaDardha "Training:PhD Course on Computational Ontologies @ University of Bologna 2011/Ontology Testing/OrnelaDardha")
* [Arefnia Scarlato](http://ontologydesignpatterns.org/wiki/Training:PhD_Course_on_Computational_Ontologies_%40_University_of_Bologna_2011/Ontology_Testing/ArefniaScarlato "Training:PhD Course on Computational Ontologies @ University of Bologna 2011/Ontology Testing/ArefniaScarlato")
* [Armir Bujari](http://ontologydesignpatterns.org/wiki/Training:PhD_Course_on_Computational_Ontologies_%40_University_of_Bologna_2011/Ontology_Testing/ArmirBujari "Training:PhD Course on Computational Ontologies @ University of Bologna 2011/Ontology Testing/ArmirBujari")
* [Yadary Ortega](http://ontologydesignpatterns.org/wiki/index.php?title=Training:PhD_Course_on_Computational_Ontologies_%40_University_of_Bologna_2011/Ontology_Testing/YadaryOrtega&action=edit&redlink=1 "Training:PhD Course on Computational Ontologies @ University of Bologna 2011/Ontology Testing/YadaryOrtega (not yet written)")
* [Antonio D'agata](http://ontologydesignpatterns.org/wiki/Training:PhD_Course_on_Computational_Ontologies_%40_University_of_Bologna_2011/Ontology_Testing/AntonioD%27agata "Training:PhD Course on Computational Ontologies @ University of Bologna 2011/Ontology Testing/AntonioD'agata")


Assume that the ontology was constructed with the following context in mind, and use the three methods described above to test the ontology. 


__Context:__ An online music database wishes to semantically represent their data about musicians, albums, and performances, in order to be able to provide better search functions to their users, i.e. by querying the knowledge base instead of using keyword-based queries. Below is an example of what they typically would like to store, and at the bottom you find the competency questions developed as requirements for the ontology.


Additionally, assume that the ontology requirements were based on the following user story:


__Story - music and bands:__ 
The current configuration of the “Red Hot Chili Peppers” is: Anthony Kiedis (vocals), Flea (bass, trumpet, keyboards, and vocals), Johs Klinghoffer (guitar), and Chad Smith (drums). 
The line-up has changed a few times during they years, Frusciante replaced Hillel Slovak in 1988, while Jack Irons was replaced by Chad Smith. 
In addition to playing guitars for Red hot Chili Peppers Frusciante also contributed to the band “The Mars Volta” as a vocalist for some time. 
In 2004, the Red Hot Chili Peppers started recording the album “Stadium Arcadium”. The album contains 28 tracks and was released in 2006. 
It includes a track of the song “Hump de Bump”, a funk-rock song composed in 2004. 


For testing you need the ontological requirements that were the basis of the ontology development, they can be found below. 
Consider that it is against these requirements that you are performing the testing, the scenario and context above only gives you some background information.
Also consider that you do not have to modify the ontology during this exercise, your goal is to identify modeling mistakes and document them. 


__Competency questions (CQs) and contextual statements of music and bands__



1. What instruments does a certain person play?
2. Who were the members of a band in a point in time?
3. What role does a certain person have in a certain band at a certain point in time?
4. What tracks are recordings of a certain song?
5. What is the genre, e.g., rock or pop, of this track?
6. What are the genres of this album?
7. During what time period was a certain album of a certain band recorded?
8. Who did participate in the recording of a certain album of a certain band?
9. When was a certain album released?
10. When was a certain song composed?


Contextual statement:



1. A recorded album has one or more genres
2. A track has only one genre
3. A track realizes only one song
4. Each band and each person is associated to at least one name


Reasoning requirement:



1. To identify (classify) bands into (multiple) genres based on the genres of their recorded tracks, e.g., a rock band has recorded some track in the genre "rock". In this system a band should be classified into a certain genre even if it has only one track of this genre.
2. To infer the genres of an album based on the genres of the tracks it contains




Retrieved from "[http://ontologydesignpatterns.org/wiki/Training:PhD\_Course\_on\_Computational\_Ontologies\_%40\_University\_of\_Bologna\_2011/Ontology\_Testing:Unrestricted\_testing](../../../Training/PhD_Course_on_Computational_Ontologies_@_University_of_Bologna_2011/Ontology_Testing/Unrestricted_testing.md)"