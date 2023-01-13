Problems in musicindustry.owl



* CQ2: The end time is missing.
	+ The query you would like to be able to write:



```
  SELECT ?band ?member ?start ?end
  WHERE {
     ?x :band ?band .
     ?x :member ?member .
     ?x :membershipStartDate ?start .
     ?x :membershipEndDate ?end
  } 

```

* + But the end date property is missing, hence the only thing we can write is:



```
  SELECT ?band ?member ?start
  WHERE {
     ?x :band ?band .
     ?x :member ?member .
     ?x :membershipStartDate ?start 
  } 

```

* CQ3: roles are not time-indexed, they are asserted through specific properties, e.g. bassPlayerOf
	+ We would need to add a new class (according to the n-ary relation pattern) representing the situation of a person playing a role in a band, and then relate the situation to a band, a person, a role and a time interval.
* CS4: missing name property for persons, Anthony Kiedis is using the property for bands and is inferred to be a band. Also missing the contextual statement that implies cardinality restrictions on people and bands, on the hasName property.
	+ Either add Person to the domain of the property (Band or Person) or add a new datatype property that has the domain Person and range xsd:string.
* Ontology is inconsistent because the domain of releaseDate is the intersection of Album and Track instead of the union.
	+ The domain should be Album or Track (in TopBraid "or" means union, while adding two separate domains mean intersection).
* A track realising "some" song doesn't mean only one!
	+ We should add a restriction on the Track, under rdfs:SubClassOf: recordingOf exactly 1
* Definition of PopBand should be "equivalent class" instead of subclass restriction
	+ Equivalence class restrictions allows us to infer class membership, i.e. perform classification of instances, so it should be something that identifies instances of that class. This is exactly what our reasoning requirement says we should be able to do.
* The second reasoning requirement is missing, hence we cannot infer the genre of an album
	+ Can be done with an OWL 2 property chain.
* Some missing domains and ranges, missing annotations etc.




Retrieved from "[http://ontologydesignpatterns.org/wiki/Training:Advanced\_Ontology\_Engineering\_at\_FOI\_-\_2011/Ontology\_Testing/Testing\_Solution](../../../Training/Advanced_Ontology_Engineering_at_FOI_-_2011/Ontology_Testing/Testing_Solution)"