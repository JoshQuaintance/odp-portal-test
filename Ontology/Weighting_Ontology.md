Return to [Catalogue of Exemplary Ontologies](../Ontology/Main "Ontology:Main")



#  Ontology Overview


#  Long Description


The Weighting Ontology includes a general multiple purpose weight concept. This concept can be used to associate any concept to a wo:Weight instance(s) with the property wo:weight. The second property of wo:Weight is wo:weight\_value, which is a simple xsd:decimal based datatype property to associate the numeric value of the weighting.
Furthermore, this ontology includes a wo:Scale, which is modeled as a sub class of scovo:Dimension to relate it to its specified scovo:Item based concept (wo:Weight) via wo:scale. To define the range of this scale the properties wo:min\_weight and wo:min\_weight can be used. These are sub properties of the related minimum and maximum properties of the Statistical Core Vocabulary (scovo:min and scovo:max) and the Review Vocabulary (rev:minRating and rev:maxRating). Finally one can define a step size (wo:step\_size) for the weighting scales.



#  Additional Information


  



  




#  References


[Add a reference](index.php@title=Odp%253AAdd_reference&subject=Ontology%253AWeighting+Ontology.html "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_reference&subject=Ontology%3AWeighting+Ontology")


  






Retrieved from "[http://ontologydesignpatterns.org/wiki/Ontology:Weighting\_Ontology](../Ontology/Weighting_Ontology)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [Ontology](../Category/Ontology "Category:Ontology")