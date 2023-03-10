[![](../images/thumb/b/b5/Certified.png/70px-Certified.png)](../Image/Certified.png "Certified.png") __This pattern has been certified.__
Related submission, with evaluation history, can be found __here__





#  Graphical representation


__Diagram__
_(this article has no graphical representation)_



#  General description


  




#  Elements


_The __LinnaeanTaxonomy__ Content OP locally defines the following ontology elements:_



[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif "ObjectProperty") __hasDirectHigherRank__ (owl:ObjectProperty) This property relates two taxa, where the first is more specific then the second and there is no other taxon that is both more general than the first and more specific than the second. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[hasDirectHigherRank](../Submissions/LinnaeanTaxonomy/hasDirectHigherRank "Submissions:LinnaeanTaxonomy/hasDirectHigherRank") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif "ObjectProperty") __hasDirectLowerRank__ (owl:ObjectProperty) This property relates two taxa, where the first is less specific then the second and there is no other taxon that is both more specific than the first and more general than the second. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[hasDirectLowerRank](../Submissions/LinnaeanTaxonomy/hasDirectLowerRank "Submissions:LinnaeanTaxonomy/hasDirectLowerRank") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif "ObjectProperty") __hasHigherRank__ (owl:ObjectProperty) This property relates two taxa, where the first is more specific than the second. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[hasHigherRank](../Submissions/LinnaeanTaxonomy/hasHigherRank "Submissions:LinnaeanTaxonomy/hasHigherRank") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif "ObjectProperty") __hasLowerRank__ (owl:ObjectProperty) This property relates two taxa, where the first is less specific than the second. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[hasLowerRank](../Submissions/LinnaeanTaxonomy/hasLowerRank "Submissions:LinnaeanTaxonomy/hasLowerRank") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif "Class") __Class__ (owl:Class) Class is the third highest traditional taxon. E.g., in the case of humans the class is 'Mammalia'. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[Class](../Submissions/LinnaeanTaxonomy/Class "Submissions:LinnaeanTaxonomy/Class") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif "Class") __Family__ (owl:Class) Family is the fifth highest traditional taxon. E.g., in the case of humans the family is 'Hominidae'. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[Family](../Submissions/LinnaeanTaxonomy/Family "Submissions:LinnaeanTaxonomy/Family") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif "Class") __Genus__ (owl:Class) Genus is the sixth highest traditional taxon. E.g., in the case of humans the genus is 'Homo'. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[Genus](../Submissions/LinnaeanTaxonomy/Genus "Submissions:LinnaeanTaxonomy/Genus") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif "Class") __Kingdom__ (owl:Class) Kingdom is the highest traditional taxon. E.g., in the case of humans the kingdom is 'Animalia'. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[Kingdom](../Submissions/LinnaeanTaxonomy/Kingdom "Submissions:LinnaeanTaxonomy/Kingdom") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif "Class") __Order__ (owl:Class) Order is the fourth highest traditional taxon. E.g., in the case of humans the phylum is 'Primates'. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[Order](../Submissions/LinnaeanTaxonomy/Order "Submissions:LinnaeanTaxonomy/Order") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif "Class") __Phylum__ (owl:Class) Phylum is the second highest traditional taxon. E.g., in the case of humans the phylum is 'Chordata'. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[Phylum](../Submissions/LinnaeanTaxonomy/Phylum "Submissions:LinnaeanTaxonomy/Phylum") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif "Class") __Species__ (owl:Class) Species is the lowest traditional taxon. E.g., in the case of humans the species is 'Homo sapiens'. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[Species](../Submissions/LinnaeanTaxonomy/Species "Submissions:LinnaeanTaxonomy/Species") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif "Class") __Taxon__ (owl:Class) A taxon is a concept denoting a type of organism or of a group of organisms. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[Taxon](../Submissions/LinnaeanTaxonomy/Taxon "Submissions:LinnaeanTaxonomy/Taxon") page_
#  Additional information


The linnaean taxonomy content ontology design pattern represents the layered classification invented by Linneus in the XVIII century. It is created by reengineering Wikipedia articles about taxa, taxonomic ranks, and linnaean taxonomy.



#  Scenarios



__Scenarios about LinnaeanTaxonomy__
No scenario is added to this Content OP.




#  Reviews



__Reviews about LinnaeanTaxonomy__
This revision (revision ID __9097__) takes in account the reviews: none


Other info at [evaluation tab](http://ontologydesignpatterns.org/wiki/index.php?title=Submissions:LinnaeanTaxonomy&action=evaluation "http://ontologydesignpatterns.org/wiki/index.php?title=Submissions:LinnaeanTaxonomy&action=evaluation")




  




#  Modeling issues



__Modeling issues about LinnaeanTaxonomy__
There is no Modeling issue related to this proposal.




  




#  References


[Add a reference](index.php@title=Odp%253AAdd_reference&subject=../Submissions/LinnaeanTaxonomy "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_reference&subject=Submissions%3ALinnaeanTaxonomy")


  






Retrieved from "[http://ontologydesignpatterns.org/wiki/Submissions:LinnaeanTaxonomy](../Submissions/LinnaeanTaxonomy)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [ProposedContentOP](../Category/ProposedContentOP "Category:ProposedContentOP")