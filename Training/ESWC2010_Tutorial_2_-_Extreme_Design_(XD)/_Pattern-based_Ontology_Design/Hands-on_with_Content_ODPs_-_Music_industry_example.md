__Problem__:
Develop an OWL ontology starting from the below use case. Note that the text is only there to help you understand the domain and the context of the ontology, but the actual modelling requirements are the competency questions and the contextual statement. 




```
  __Note:__ Treat the CQs and the contextual statement as the 
  requirements of your model. The result of your modelling should represent these, but also conform to 
  the modelling "best practices" that have been taught in the course, e.g. appropriate naming of concepts.
  Use the XD methodology as a guideline for your work, and the steps you should perform.

```

  

__Context__


An online music database wishes to semantically represent their data about musicians, albums, and performances, in order to be able to provide better search functions to their users, i.e. by querying the knowledge base instead of using keyword queries. Below is an example of what they typically would like to store, and at the bottom you find the competency questions developed as requirements for the ontology.


  

__Story: music and bands__


The current configuration of the “Red Hot Chili Peppers” are: Anthony Kiedis (vocals), Flea (bass, trumpet, keyboards, and vocals), John Frusciante (guitar), and Chad Smith (drums). The line-up has changed a few times during they years, Frusciante replaced Hillel Slovak in 1988, and when Jack Irons left the band he was briefly replaced by D.H. Peligo until the band found Chad Smith. In addition to playing guitars for Red hot Chili Peppers Frusciante also contributed to the band “The Mars Volta” as a vocalist for some time.


From September 2004, the Red Hot Chili Peppers started recording the album “Stadium Arcadium”. The album contains 28 tracks and was released on May 5 2006. It includes a track of the song “Hump de Bump”, which was composed in January 26, 2004. The critic Crian Hiatt defined the album as "the most ambitious work in his twenty-three-year career". On August 11 (2006) the band gave a live performance in Portland, Oregon (US), featuring songs from Stadium Arcadium and other albums.


  

__Competency questions (CQs) and contextual statements of music and bands__




```
  1. What instruments does a certain person play?
  2. What are the members of a certain band during a certain time period?
  3. What role does a certain person have in a certain band during a certain time?
  4. During what time period was a certain album recorded?
  5. How many tracks does a particular album contain?
  6. When was a certain album released?
  7. What song is a specific track a recording of?
  8. When was a certain song composed?
  9. What does a certain critic say about a certain album?
 10. When did a certain performance take place?
 11. What songs were played in a certain performance?
 12. Where did a certain performance take place?
 13. In what region is a certain city located?
 14. In what country is a certain region located?

```


```
  __Contextual statement:__
  1. An album always contains at least one track.

```

  

__XD Methodology - reminder__


Relevant tasks for the exercise are in bold face.



* Task 1 – Familiarize with the domain and task
* Task 2 – Collect requirements stories
* Task 3 – Select a story
* Task 4 – Transform the story into CQs
* __Task 5 – Select a CQ__
* __Task 6 – Match CQs to GUCs of [Content ODPs](../../../Submissions/ContentOPs "Submissions:ContentOPs")__
* __Task 7 – Select the Content ODPs to reuse__
* __Task 8 – Reuse and integrate selected Content ODPs__
	+ Import
	+ Specialize
	+ Extend
	+ Integrate
* __Task 9 – Test and fix (run SPARQL queries with test instances)__
* Task 10 – Release module
* __Task 11 – Integrate, test and fix__
* Task 12 – Release new version of the ontology



__Solutions__:





Retrieved from "[http://ontologydesignpatterns.org/wiki/Training:ESWC2010\_Tutorial\_2\_-\_Extreme\_Design\_%28XD%29:\_Pattern-based\_Ontology\_Design/Hands-on\_with\_Content\_ODPs\_-\_Music\_industry\_example](../../../Training/ESWC2010_Tutorial_2_-_Extreme_Design_(XD)/_Pattern-based_Ontology_Design)/_Pattern-based_Ontology_Design.md)/_Pattern-based_Ontology_Design/Hands-on_with_Content_ODPs_-_Music_industry_example.md)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [Exercise](../../../Category/Exercise "Category:Exercise")