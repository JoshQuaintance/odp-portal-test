There can be alternative solutions, however, one possible set of ODPs could be:



* CQs 1-3 + contextual statement:  [Situation](../../../Submissions/Situation.md "Submissions:Situation") - The festival is a specialization of a Situation, and in its setting there is a place, a time, and a number of plays (connected by specializing the hasSetting/isSettingFor properties + restrictions on the festival class).
* CQs 4-5:  [Place](../../../Submissions/Place.md "Submissions:Place") - Both cities and countries are places, and the hasLocation/isLocationOf properties can be used for both these cases + restrictions on the classes, e.g. so that cities cannot be located in other cities but only in countries etc. In addition the pattern specialization needs to be extended with a theater class.
* CQ 6 + contextual statement:  [Information realization](../../../Submissions/Information_realization.md "Submissions:Information realization") - The production can be seen as a concrete realization of the abstract play, and each production is the realization of exactly one play.
* CQ 7:  [Time interval](../../../Submissions/TimeInterval.md "Submissions:TimeInterval") - Creating an instance of a time interval class, rather than just two literal values allows us to talk about the interval as such, and set restrictions on it, e.g. that each play is written during exactly one interval, and that interval in turn has exactly one start and one end point.
* CQ 8, 9, 10:  [Situation](../../../Submissions/Situation.md "Submissions:Situation") - Again, these CQs can each be seen as a "situation", i.e. an n-ary relation, with several things involved in the setting. In fact, we need them to be modeled in this way in order to be able to distinguish the particular combination of parameters.




Retrieved from "[http://ontologydesignpatterns.org/wiki/Training:Advanced\_Ontology\_Engineering\_at\_FOI\_-\_2011/Ontology\_Design\_Patterns/Solution\_Ideas](../../../Training/Advanced_Ontology_Engineering_at_FOI_-_2011/Ontology_Design_Patterns/Solution_Ideas.md)"