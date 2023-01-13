Return to [Catalogue of Exemplary Ontologies](../Ontology/Main "Ontology:Main")



#  Ontology Overview


#  Long Description


The Association Ontology combines features of the Similarity Ontology, the Review Ontology and DCMI Metadata Terms. The intend behind this ontology is to provide a mechanism to append (personal) association statements (sim:Association) to something by using the relation sim:association. This step of indirection is neccessary to enable:




```
   * reusable association statements and
   * voting, rating and reviewing of association statements in a specific context.

```

Therefore, the sub class ao:LikeableAssociation was created, which combines the concepts of sim:Association and rev:Review. Simple voting (the "like button") can be realized by using the property ao:likeminded, which creates a relation between an association statement and an individuum (foaf:Agent). Ratings and reviews can be realized by using the features of the Review Ontology, e.g. rev:rating or rev:Feedback.
To address associations of a specific domain, e.g. genre, mood or occasion, new sub properties based on dcterms:subject were created. These are:




```
   * ao:genre: a hook for genres descriptions of all kind,
   * ao:mood: a hook for mood descriptions and
   * ao:occasion: a hook for occasion descriptions.

```

They are intendend to be an abstact and general hook into their specific domains (genre, mood, occasion). Furthermore, new, more specific sub properties based on these properties should be created to provide a hook in more specific domains, e.g. mo:genre for music genres/styles (this sub property relation isn't currently the case).
To enable voting, rating and reviewing of a reusable association statements in a specific context, the property ao:included\_association was created. By using this relation one can include a reusable association statement into another association statement (preferable based on ao:LikeableAssociation). Please have also a look at the example in this document, which illstrates this use case.



#  Additional Information


  



  




#  References


[Add a reference](index.php@title=Odp%253AAdd_reference&subject=Ontology%253AAssociation+Ontology.html "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_reference&subject=Ontology%3AAssociation+Ontology")



* A blog post about the Association Ontology with examples and graphics. [Weblog post](http://smiy.org/2010/07/26/the-association-ontology/ "http://smiy.org/2010/07/26/the-association-ontology/") | [reference page](../Community/References/Association_Ontology_announcement "Community:References/Association Ontology announcement")




Retrieved from "[http://ontologydesignpatterns.org/wiki/Ontology:Association\_Ontology](../Ontology/Association_Ontology)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [Ontology](../Category/Ontology "Category:Ontology")