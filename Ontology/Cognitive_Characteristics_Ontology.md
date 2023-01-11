Return to [Catalogue of Exemplary Ontologies](../Ontology/Main.md "Ontology:Main")



#  Ontology Overview


#  Long Description


The Cognitive Characteristics Ontology includes two opportunities to model cognitive patterns. The first one is the representation of cognitive characteristics by using the semantic relation cco:cognitive\_characteristic or better its more specialised sub properties (see graphic cco:cognitive\_characteristic property as graph with relations) to associate the topics of the cognitive patterns to the users. The second opportunity is the property-oriented context reification of cco:cognitive\_characteristic, cco:CognitiveCharacteristic, which is a general multiple purpose cognitive characteristic concept to describe cognitive patterns more in detail for a specific user or user group.
As one can see in graphic cco:CognitiveCharacteristic concept as graph with relations, the specialised sub properties of cco:cognitive\_characteristic, the cognitive patterns, currently are




```
   * interest (cco:interest), that means, a certain area of interest or preference, which is equivalent to foaf:topic_interest,
   * compentence (cco:competence), that means, the compentence to (be able to) do or know something or
   * setting (cco:setting), often regarding a specific environment, e.g. an application.

```

One can also refine the semantic relation of a competence association by using the sub properties of cco:competence, which are currently:




```
   * cco:skill: the ability or skill to (be able to) do something, e.g. to walk, to play the piano or to work in a team
   * cco:expertise: the knowledge or expertise in a certain domain or a specific topic, e.g. football, programming languages or music
   * cco:belief: an uncertain relation for competence representation, that means beliefs, persuasions or opinions, which can also be misconceptions

```

One can see the second opportunity to model cognitive patterns, cco:CognitiveCharacteristic in graphic cco:CognitiveCharacteristic concept as simplified graph with relations. This concept can be used to associate any foaf:Agent instance to (a) cco:CognitiveCharacteristic instance(s) with help of the properties cco:habit and cco:agent. The topics of a cco:CognitiveCharacteristic instance are related to it by using the property cco:topic, so that a property chain of cco:habit and cco:topic will also direct to topics of a cognitive pattern of an user or user group. That means, a statement that is modelled with the simple semantic relation approach based on cco:cognitive\_characteristic can also be represented by an instance of cco:CognitiveCharacteristic, which has a cco:agent or cco:habit, a cco:topic and a cco:characteristic relation. The last property in this row is used to associate the applied cognitive pattern relation (sub properties of cco:cognitive\_characteristic).
Different statistics can be made on cognitive characteristics. These are currently:




```
   * cco:overall_weight, which reflects the overall interest in a topic and should be different from the actual weight (associated by the property wo:weight) of a cognitive characteristic
   * cco:longest_duration, which is the longest continuous interval of attention for a cognitive pattern, e.g. for an interest, if it appears in the following years: 1990, 1991, 1995, 1996, 1997, 1998, 2001, then the longest duration is 4 years
   * cco:ultimative_duration, which is the overall duration of attention for a cognitive pattern, e.g. for an interest, if it appears in the following years: 1990, 1991, 1995, 1996, 1997, 1998, 2001, then the longest duration is 7 years

```

Besides these statistics, one can also associate a concrete activity (by using the property cco:activity), to differentiate e.g. between football playing (topic = football; activity = playing) and football watching (topic = football; activity = watching), and further statistical items (by using the property cco:statistical\_item) to a cognitive pattern description, which is itself also a sub class of scovo:Item.
It is also important, to be able to describe dynamics of a cognitive characteristic. In the Cognitive Characteristics Ontology they can be described with help of the cco:CharacteristicDynamics concept, which is a sub class of wo:Weight, and can be related to a cco:CognitiveCharacteristic instance by using the property cco:characteristic\_dynamics. Thereby, one can relate




```
   * concrete appear times (time instants or intervals, by using the property cco:appear_time), when a cognitive pattern gets attention by someone, or
   * an evidence description (by using the property cco:evidence), where this characteristic or dynamics was derived from.

```

to a cco:CognitiveCharacteristic or cco:characteristic\_dynamics instance.
Due to the two modelling opportunities of cognitive pattern in the Cognotive Characteristics Ontology, there is a need for formal semantics to associate statements with a shortcut relation and instances of the reification class that belonging together or to infer such knowledge with a reasoning engine. The Property Reification Vocabulary fulfil these requirements.



#  Additional Information


  



  




#  References


[Add a reference](index.php@title=Odp%253AAdd_reference&subject=Ontology%253ACognitive+Characteristics+Ontology.html "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_reference&subject=Ontology%3ACognitive+Characteristics+Ontology")



* A blog post about the Cognitive Characteristics Ontology with examples and graphics. [Weblog post](http://smiy.org/2010/10/19/the-cognitive-characteristics-ontology/ "http://smiy.org/2010/10/19/the-cognitive-characteristics-ontology/") | [reference page](../Community/References/Cognitive_Characteristics_Ontology_annoucement.md "Community:References/Cognitive Characteristics Ontology annoucement")




Retrieved from "[http://ontologydesignpatterns.org/wiki/Ontology:Cognitive\_Characteristics\_Ontology](../Ontology/Cognitive_Characteristics_Ontology.md)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [Ontology](../Category/Ontology.md "Category:Ontology")