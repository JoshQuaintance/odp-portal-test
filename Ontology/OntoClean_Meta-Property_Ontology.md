Return to [Catalogue of Exemplary Ontologies](../Ontology/Main.md "Ontology:Main")



#  Ontology Overview


#  Long Description


The axiomitization of OntoClean in S5 modal logic entails certain constraints between classes in a taxonomy. These constraints are well within the expressive power of OWL, given the ability to view the \*classes\* as an "abox" and declare their metaproperties using the rdf:type relation. One very simple way to accomplish this, is to take the OWL version of an ontology, and in a text editor replace owl:class with "[http://www.ontoclean.org/ontoclean-dl-v1.owl#Class](http://www.ontoclean.org/ontoclean-dl-v1.owl#Class "http://www.ontoclean.org/ontoclean-dl-v1.owl#Class")", and import this ontology. Then add the rdf:type relations to indicate which classes are rigid, dependent, etc. Any OWL reasoner will be able to find inconsistencies in the taxonomy as a result.



#  Additional Information


  



  




#  References


[Add a reference](index.php@title=Odp%253AAdd_reference&subject=Ontology%253AOntoClean+Meta-Property+Ontology.html "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_reference&subject=Ontology%3AOntoClean+Meta-Property+Ontology")



* SemanticWeb.org Wiki article [Documentation](http://semanticweb.org/wiki/OntoClean "http://semanticweb.org/wiki/OntoClean") | [reference page](../Community/References/OntoClean_Wiki_Entry.md "Community:References/OntoClean Wiki Entry")
* Wikipedia article [Documentation](http://en.wikipedia.org/wiki/Ontoclean "http://en.wikipedia.org/wiki/Ontoclean") | [reference page](../Community/References/OntoClean_Wikipedia_article.md "Community:References/OntoClean Wikipedia article")




Retrieved from "[http://ontologydesignpatterns.org/wiki/Ontology:OntoClean\_Meta-Property\_Ontology](../Ontology/OntoClean_Meta-Property_Ontology.md)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [Ontology](../Category/Ontology.md "Category:Ontology")