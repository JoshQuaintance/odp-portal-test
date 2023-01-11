Return to [Catalogue of Exemplary Ontologies](../Ontology/Main.md "Ontology:Main")



#  Ontology Overview


#  Long Description


The Recommendation Ontology is an ontology for modeling high level recommendations on/ for the Semantic Web. Thereby, the ontology hook up parts of the Similarity Ontology, DCMI Metadata Terms, the Association Ontology and the Ordered List Ontology.
The core of the Recommendation Ontology is the rec:Recommendation concept. A rec:Recommendation instance can consist of




```
   * an item or agent relation (rec:Recommendation or its inverse property rec:for) to associate the resource, for which the recommendation was made
   * an recommender relation (rec:recommender or its inverse property rec:recommends) to associate the instance, which provided or calculated the recommendation, e.g. an is:InfoService instance
   * recommendation object relations (rec:recommendation_object or its inverse property rec:recommended_in) to associate appropriated objects to the recommendation subject
   * recommendation audience relations (rec:recommendation_audience to associate groups or stereotypes, which are probably appropriated as target group for this recommendation.

```

Since rec:Recommendation is a sub class of ao:LikeableAssociation, it is also possible to like (ao:likeminded), rate (rev:rating) or give a feedback (rev:Feedback) to a recommendation. Furthermore, one can also relate detailed association (sim:Association) or similarity statements (sim:Similarity) to a recommendation by using the property ao:included\_association.
As an extension of rec:Recommendation, we built the rec:RankedRecommendation concept to enable also ordered (ranked) recommendations at a high level. rec:RankedRecommendation is not only a sub class of rec:Recommendation. Furthermore, it is also a sub class of olo:OrderedList, which enables all features of an ordered list also to this concept. Following this design, a rec:ranked\_recommendation is not only a sub property of rec:recommendation\_object, but also a sub property of olo:slot. That means the recommendation objects are now related by using the property olo:item.



#  Additional Information


  



  




#  References


[Add a reference](index.php@title=Odp%253AAdd_reference&subject=Ontology%253ARecommendation+Ontology.html "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_reference&subject=Ontology%3ARecommendation+Ontology")



* A blog post about the Recommendation Ontology with examples and graphics. [Weblog post](http://smiy.org/2010/08/07/the-recommendation-ontology/ "http://smiy.org/2010/08/07/the-recommendation-ontology/") | [reference page](../Community/References/Recommendation_Ontology_announcement.md "Community:References/Recommendation Ontology announcement")




Retrieved from "[http://ontologydesignpatterns.org/wiki/Ontology:Recommendation\_Ontology](../Ontology/Recommendation_Ontology.md)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [Ontology](../Category/Ontology.md "Category:Ontology")