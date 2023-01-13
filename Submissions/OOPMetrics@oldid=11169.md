[![](../images/thumb/b/b5/Certified.png/70px-Certified.png)](../Image/Certified.png "Certified.png") __This pattern has been certified.__
Related submission, with evaluation history, can be found __here__





#  Graphical representation


__Diagram__




[![Image:OOPMetrics.png](../images/a/a2/OOPMetrics.png)](../Image/OOPMetrics.png "Image:OOPMetrics.png")




#  General description


  




#  Elements


_The __OOPMetrics__ Content OP locally defines the following ontology elements:_



[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif "ObjectProperty") __hasClass__ (owl:ObjectProperty) Refers to an OOPClass from an OOPPackage.
  



Se refera la o OOPClass dintr-un OOPPackage. 



 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[hasClass](../Submissions/OOPMetrics/hasClass "Submissions:OOPMetrics/hasClass") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif "ObjectProperty") __hasMethod__ (owl:ObjectProperty) Refers to an OOPMethod from an OOPClass.
  



Se refera la o OOPMethod dintr-o OOPClass. 



 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[hasMethod](../Submissions/OOPMetrics/hasMethod "Submissions:OOPMetrics/hasMethod") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif "ObjectProperty") __hasMetric__ (owl:ObjectProperty) Refers to a software metric that an OOPProject/OOPPackage/OOPClass/OOPMethod has.
  



Se refera la o metrica soft pe care o are un/o OOPProject/OOPPackage/OOPClass/ OOPMethod. 



 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[hasMetric](../Submissions/OOPMetrics/hasMetric "Submissions:OOPMetrics/hasMetric") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif "ObjectProperty") __hasPackage__ (owl:ObjectProperty) Refers to an OOPPackage from an OOPProject.
  



Se refera la un OOPPackage dintr-un OOPProject. 



 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[hasPackage](../Submissions/OOPMetrics/hasPackage "Submissions:OOPMetrics/hasPackage") page_
[![DatatypeProperty](../images/thumb/a/a5/DatatypeProperty.gif/20px-DatatypeProperty.gif)](../Image/DatatypeProperty.gif "DatatypeProperty") __hasFloatValue__ (owl:DatatypeProperty) The real value of the software metric.
  



Valoarea reala pentru metrica soft. 



 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[hasFloatValue](../Submissions/OOPMetrics/hasFloatValue "Submissions:OOPMetrics/hasFloatValue") page_
[![DatatypeProperty](../images/thumb/a/a5/DatatypeProperty.gif/20px-DatatypeProperty.gif)](../Image/DatatypeProperty.gif "DatatypeProperty") __hasIntegerValue__ (owl:DatatypeProperty) The integer value of the software metric.
  



Valoarea intreaga pentru metrica soft. 



 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[hasIntegerValue](../Submissions/OOPMetrics/hasIntegerValue "Submissions:OOPMetrics/hasIntegerValue") page_
[![DatatypeProperty](../images/thumb/a/a5/DatatypeProperty.gif/20px-DatatypeProperty.gif)](../Image/DatatypeProperty.gif "DatatypeProperty") __hasName__ (owl:DatatypeProperty) This represents the name (more precisely the acronym) of the category of software metric. Such as: "WMC" for "Weighted Methods Count", TCC for "Tight Class Cohesion", etc.
  



Aceasta reprezinta numele (mai precis acronimul) pentru categoria de metrica soft. Cum ar fi: "WMC" pentru "Weighted Methods Count", TCC pentru "Tight Class Cohesion", etc. 



 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[hasName](../Submissions/OOPMetrics/hasName "Submissions:OOPMetrics/hasName") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif "Class") __OOPClass__ (owl:Class) This represents the "class" concept from object-oriented programming.
  



Aceasta reprezinta conceptul "clasa" din programarea orientata obiect. 



 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[OOPClass](../Submissions/OOPMetrics/OOPClass "Submissions:OOPMetrics/OOPClass") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif "Class") __OOPMethod__ (owl:Class) This represents the "method" concept from object-oriented programming.
  



Aceasta reprezinta conceptul "metoda" din programarea orientata obiect. 



 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[OOPMethod](../Submissions/OOPMetrics/OOPMethod "Submissions:OOPMetrics/OOPMethod") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif "Class") __OOPMetric__ (owl:Class) This represents a software metric specific to object-oriented programming.
  



Aceasta reprezinta o metrica soft specifica programarii orientate obiect. 



 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[OOPMetric](../Submissions/OOPMetrics/OOPMetric "Submissions:OOPMetrics/OOPMetric") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif "Class") __OOPPackage__ (owl:Class) This represents the "package" concept from object-oriented programming.
  



Aceasta reprezinta conceptul "pachet" din programarea orientata obiect. 



 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[OOPPackage](../Submissions/OOPMetrics/OOPPackage "Submissions:OOPMetrics/OOPPackage") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif "Class") __OOPProject__ (owl:Class) This represents a software project.
  



Aceasta reprezinta un proiect soft. 



 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[OOPProject](../Submissions/OOPMetrics/OOPProject "Submissions:OOPMetrics/OOPProject") page_
#  Additional information


Note from the author to the evaluators:
the title of the related article is: "An Ontology Pattern for Software Metrics", submission 21.



#  Scenarios



__Scenarios about OOPMetrics__
No scenario is added to this Content OP.




#  Reviews



__Reviews about OOPMetrics__
This revision (revision ID __11169__) takes in account the reviews: [MariaPoveda about OOPMetrics](../Reviews/MariaPoveda_about_OOPMetrics "Reviews:MariaPoveda about OOPMetrics"), [RinkeHoekstra about OOPMetrics](../Reviews/RinkeHoekstra_about_OOPMetrics "Reviews:RinkeHoekstra about OOPMetrics")


Other info at [evaluation tab](http://ontologydesignpatterns.org/wiki/index.php?title=Submissions:OOPMetrics&action=evaluation "http://ontologydesignpatterns.org/wiki/index.php?title=Submissions:OOPMetrics&action=evaluation")




  




#  Modeling issues



__Modeling issues about OOPMetrics__
There is no Modeling issue related to this proposal.




  




#  References


[Add a reference](index.php@title=Odp%253AAdd_reference&subject=../Submissions/OOPMetrics "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_reference&subject=Submissions%3AOOPMetrics")


  






Retrieved from "[http://ontologydesignpatterns.org/wiki/Submissions:OOPMetrics](../Submissions/OOPMetrics)"
 [Categories](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [ProposedContentOP](../Category/ProposedContentOP "Category:ProposedContentOP") | [Submitted to event](../Category/Submitted_to_event "Category:Submitted to event") | [Review assigned](../Category/Review_assigned "Category:Review assigned")