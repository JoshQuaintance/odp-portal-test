__Problem__:
To develop an OWL ontology starting from a use case. 


__Context__


The Warner Bros recording label has decided to manage its own productions by means of an ontology-driven application. They provide the designers with documents describing scenarios that informally describe the typical objects and data to be stored in the knowledge base.
From this documents one story is extracted and assigned to ontology designers.


  

__Story for exercise 1: album production__


The “Red Hot Chili Peppers” are: Anthony Kiedis (vocals), Flea (bass, trumpet, keyboards, and vocals), John Frusciante (guitar), and Chad Smith (drums). During 2005, the band recorded the album “Stadium Arcadium”. The album contains 28 tracks and has been released in May 2006. It includes the track of the song “Hump de Bump”, which was composed in January 2004. The critic Crian Hiatt defines the album as "the most ambitious work in his twenty-three-year career".


The phrase above can be simplified by transforming it into 5 sentences:



* __s1__: The “Red Hot Chili Peppers” are: Anthony Kiedis (vocals), Flea (bass, trumpet, keyboards, and vocals), John Frusciante (guitar), and Chad Smith (drums).
* __s2__: During 2005, the band recorded the album “Stadium Arcadium”.
* __s3__: The album contains 28 tracks, and has been released in May 2006.
* __s4__: It includes the track of the song “Hump de Bump”, which was composed in January 2004.
* __s5__: The critic Crian Hiatt defines the album as "the most ambitious work in his twenty-three-year career".



__Solutions__:



* [Download a possible OWL ontology that solves the exercise](http://www.ontologydesignpatterns.org/cpont/sssw08-music-production.owl "http://www.ontologydesignpatterns.org/cpont/sssw08-music-production.owl")


###   Simple sentences of _album production_ story


* __s1__: The “Red Hot Chili Peppers” are: Anthony Kiedis (vocals), Flea (bass, trumpet, keyboards, and vocals), John Frusciante (guitar), and Chad Smith (drums).
* __s2__: During 2005, the band recorded the album “Stadium Arcadium”.
* __s3__: The album contains 28 tracks, and has been released in May 2006.
* __s4__: It includes the track of the song “Hump de Bump”, which was composed in January 2004.
* __s5__: The critic Crian Hiatt defines the album as "the most ambitious work in his twenty-three-year career".


###   Instance-free sentences of _album production_ story


* __instance-free s1__:


1. Band members are persons
2. A person has a role
3. A person can play an instrument


* __instance-free s2__:


1. Members of a band record an album at a certain time interval


* __instance-free s3__:


1. A recorded album contains tracks and is released at a certain time interval.


* __instance-free s4__:


1. Songs are composed at a certain time and recorded as tracks at a certain time.


* __instance-free s5__:


1. A critique by a Person about an album has a text.


###   Selected CPs for _album production_ story


* [situation](http://www.ontologydesignpatterns.org/cp/owl/situation.owl "http://www.ontologydesignpatterns.org/cp/owl/situation.owl")
* [partof](http://www.ontologydesignpatterns.org/cp/owl/partof.owl "http://www.ontologydesignpatterns.org/cp/owl/partof.owl")
* [agent role](http://www.ontologydesignpatterns.org/cp/owl/agentrole.owl "http://www.ontologydesignpatterns.org/cp/owl/agentrole.owl")
* [object role](http://www.ontologydesignpatterns.org/cp/owl/objectrole.owl "http://www.ontologydesignpatterns.org/cp/owl/objectrole.owl")
* [classification](http://www.ontologydesignpatterns.org/cp/owl/classification.owl "http://www.ontologydesignpatterns.org/cp/owl/classification.owl")
* [collection](http://www.ontologydesignpatterns.org/cp/owl/collectionentity.owl "http://www.ontologydesignpatterns.org/cp/owl/collectionentity.owl")
* [information realization](http://www.ontologydesignpatterns.org/cp/owl/informationrealization.owl "http://www.ontologydesignpatterns.org/cp/owl/informationrealization.owl")
* [time interval](http://www.ontologydesignpatterns.org/cp/owl/timeinterval.owl "http://www.ontologydesignpatterns.org/cp/owl/timeinterval.owl")
* [album critique situation](http://www.ontologydesignpatterns.org/cp/owl/albumcritiquesituation.owl "http://www.ontologydesignpatterns.org/cp/owl/albumcritiquesituation.owl")
* [song track](http://www.ontologydesignpatterns.org/cp/owl/songtrack.owl "http://www.ontologydesignpatterns.org/cp/owl/songtrack.owl")


###   CP annotation schema


* [cp annotation schema](http://www.ontologydesignpatterns.org/schemas/cpannotationschema.owl "http://www.ontologydesignpatterns.org/schemas/cpannotationschema.owl")


###   Competency questions, unit tests


The unit tests are here substantiated as SPARQL queries.
Syntax has to be adjusted in order to comply to namespaces prefixes and ontology element names used in the actual ontology.



* __s1__
	+ __cq1__: Who are the members of a band?
	+ __cq2__: Which band a certain person is a member of?



```
  SELECT ?member ?band
  WHERE { ?member a :Person .
  ?band a :Band.
  ?band :hasBandMember ?member}

```

* + __cq3__: What roles has a certain person?
	+ __cq4__: Who has a certain role?



```
  SELECT ?person ?role
  WHERE { ?person a :Person .
  ?role a :Role.
  ?person :hasRole ?role}

```

* + __cq5__: What instruments can play a certain person?
	+ __cq6__: Who can play a certain instrument?



```
  SELECT ?person ?instrument
  WHERE { ?person a :Person .
  ?instrument a :InstrumentType.
  ?person :canPlayInstrument ?instrument}

```

* __s2__
	+ __cq7__: When has been recorded a certain album?



```
  SELECT ?album ?date  
  WHERE {?time a :TimeInterval.
  ?album a :RecordedAlbum.
  ?recording_sit a :RecordingSituation.
  ?recording_sit :hasRecordingTime ?time.
  ?time :hasRecordingDate ?date .
  ?recording_sit :forAlbum ?album}

```

* + __cq8__: Who is involved in the recording of a certain album?



```
  SELECT ?person ?album
  WHERE {?person a :Person.
  ?album a :RecordedAlbum.
  ?recording_sit a :RecordingSituation.
  ?recording_sit :forAlbum ?album.
  ?recording_sit :involvesMusician ?person}

```

* __s3__
	+ __cq9__: When was a certain album released?
	+ __cq10__: What albums have been released at a certain time interval?



```
  SELECT ?album ?date
  WHERE {?album a :RecordedAlbum.
  ?time a :TimeInterval.
  ?album :hasReleaseTime ?time.
  ?time :hasReleaseDate ?date}

```

* + __cq11__: What tracks are included in a certain album?
	+ __cq12__: What albums a certain track is contained in?



```
  SELECT ?album ?track
  WHERE {?album a :RecordedAlbum.
  ?track a :Track.
  ?album :containsTrack ?track.}

```

* + __cq13__: What tracks were produced for albums recorded at a certain time interval?



```
  SELECT ?track ?album ?date
  WHERE {?track a :Track.
  ?album a :RecordedAlbum.
  ?time a :TimeInterval.
  ?time :hasRecordingDate ?date.
  ?recording_sit :hasRecordingTime ?time.
  ?recording_sit :forAlbum ?album.
  ?recording_sit :producesTrack  ?track}

```

* __s4__
	+ __cq14__: What tracks are the recording of a certain song?



```
  SELECT ?track ?song
  WHERE {?track a :Track.
  ?song a :Song.
  ?song :songInTrack ?track}

```

* + __cq15__: When was a song composed?



```
  SELECT ?song ?date
  WHERE {?song a :Song.
  ?time a :TimeInterval.
  ?time :hasCompositionDate ?date.
  ?song :hasCompositionTime ?time}

```

* + __cq16__: When was a track recorded?



```
  SELECT ?track ?date
  WHERE {?track a :Track.
  ?time a :TimeInterval.
  ?time :hasRecordingDate ?date.
  ?recording_sit :producesTrack ?track.
  ?recording_sit :hasRecordingTime ?time}

```

* + __cq17__: When was a song recorded as a track?



```
  SELECT ?song ?track ?date
  WHERE {?song a :Song.
  ?track a :Track.
  ?time a :TimeInterval.
  ?time :hasRecordingDate ?date.
  ?song :isRealizedBy ?track.
  ?recording_sit :producesTrack ?track.
  ?recording_sit :hasRecordingTime ?time}

```

* __s5__ ->
	+ __cq17__: Who did express a critique about a certain album?
	+ __cq18__: What albums did review a certain critic?



```
  SELECT ?critic ?album
  WHERE {?critic a :Person.
  ?album a :RecordedAlbum.
  ?critique_sit :onAlbum ?album.
  ?critique_sit :byCritic ?critic}

```

* + __cq19__: What does a certain critic say about a certain album?



```
  SELECT ?critic ?album ?text
  WHERE {?critic a :Person.
  ?album a :RecordedAlbum.
  ?critique_sit :onAlbum ?album.
  ?critique_sit :byCritic ?critic.
  ?critique_sit :hasCritiqueText ?text}

```



Retrieved from "[http://ontologydesignpatterns.org/wiki/Training:NeOn\_2008\_Tutorial\_on\_Computational\_Ontologies/Music\_Industry\_Ontology](../../Training/NeOn_2008_Tutorial_on_Computational_Ontologies/Music_Industry_Ontology.md)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [Exercise](../../Category/Exercise.md "Category:Exercise")