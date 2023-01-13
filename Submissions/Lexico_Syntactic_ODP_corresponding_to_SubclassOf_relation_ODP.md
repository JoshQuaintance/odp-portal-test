[![](../images/thumb/b/b5/Certified.png/70px-Certified.png)](../Image/Certified.png.md "Certified.png") __This pattern has been certified.__
Related submission, with evaluation history, can be found __here__





#  Description


  




#  Cases


_The __Lexico Syntactic ODP corresponding to SubclassOf relation ODP__ Lexico-Syntactic ODP includes the following cases (see also [abbreviations and symbols used in LSP Formalization](../Community/LSPSymbols.md "Community:LSPSymbols")):_


  






__NL Formulation__



* An orphan drug is a type of drug.
* Odometry, speedometry and GPS are types of sensors.


__LSP Formalization__




```
[(NP<subclass>,)* and] NP<subclass> be [CN-CATV] NP<superclass>

```

__Reusable JAPE code__: [SC\_1\_2.jape](../images/c/c1/SC_1_2.jape "SC 1 2.jape")





[![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[1](../Submissions/Lexico_Syntactic_ODP_corresponding_to_SubclassOf_relation_ODP/1.md "Submissions:Lexico Syntactic ODP corresponding to SubclassOf relation ODP/1") page_





__NL Formulation__



* Prefixes and suffixes are classified as affixes.


__LSP Formalization__




```
[(NP<subclass>,)* and] NP<subclass> classify as NP<superclass>

```

__Reusable JAPE code__: [SC\_3.jape](../images/9/90/SC_3.jape "SC 3.jape")





[![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[2](../Submissions/Lexico_Syntactic_ODP_corresponding_to_SubclassOf_relation_ODP/2.md "Submissions:Lexico Syntactic ODP corresponding to SubclassOf relation ODP/2") page_





__NL Formulation__



* Thyroid medicines belong to the general group of hormone medicines.
* Starfish fall into the class Asteroidea.


__LSP Formalization__




```
[(NP<subclass>,)* and] NP<subclass> (belong to)\(fall into) CN-CATV NP<superclass>

```

__Reusable JAPE code__: [SC\_3.jape](../images/9/90/SC_3.jape "SC 3.jape")





[![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[3](../Submissions/Lexico_Syntactic_ODP_corresponding_to_SubclassOf_relation_ODP/3.md "Submissions:Lexico Syntactic ODP corresponding to SubclassOf relation ODP/3") page_





__NL Formulation__



* There are several kinds of memory: fast, expensive, short term memory, and long-term memory.


__LSP Formalization__




```
There are QUAN CN-CATV NP<superclass> PARA [(NP<subclass>,)* and] NP<subclass>

```

__Reusable JAPE code__: [SC\_4.jape](../images/5/5f/SC_4.jape "SC 4.jape")





[![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[4](../Submissions/Lexico_Syntactic_ODP_corresponding_to_SubclassOf_relation_ODP/4.md "Submissions:Lexico Syntactic ODP corresponding to SubclassOf relation ODP/4") page_





__NL Formulation__



* Some examples of peripherals are keyboards, mice, monitors, printers, scanners, disk and tape drives, microphones, speakers, joysticks, plotters and cameras.
* Types of criteria for assessing applications are: quality, safety and efficacy.


__LSP Formalization__




```
[A(n)/QUAN] example of/CN-CATV NP<superclass> be/include [PARA] [(NP<subclass>,)* and] NP<subclass>

```

__Reusable JAPE code__: [SC\_5.jape](../images/d/d5/SC_5.jape "SC 5.jape")





[![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[5](../Submissions/Lexico_Syntactic_ODP_corresponding_to_SubclassOf_relation_ODP/5.md "Submissions:Lexico Syntactic ODP corresponding to SubclassOf relation ODP/5") page_



#  Additional information


#  Reviews



__Reviews about Lexico Syntactic ODP corresponding to SubclassOf relation ODP__
There is no review about this proposal.
This revision (revision ID __8973__) takes in account the reviews: none


Other info at [evaluation tab](http://ontologydesignpatterns.org/wiki/index.php?title=Submissions:Lexico_Syntactic_ODP_corresponding_to_SubclassOf_relation_ODP&action=evaluation "http://ontologydesignpatterns.org/wiki/index.php?title=Submissions:Lexico_Syntactic_ODP_corresponding_to_SubclassOf_relation_ODP&action=evaluation")




  




#  Modeling issues



__Modeling issues about Lexico Syntactic ODP corresponding to SubclassOf relation ODP__
There is no Modeling issue related to this proposal.




  




#  References


[Add a reference](index.php@title=Odp%253AAdd_reference&subject=Submissions%253ALexico+Syntactic+ODP+corresponding+to+SubclassOf+relation+ODP.html "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_reference&subject=Submissions%3ALexico+Syntactic+ODP+corresponding+to+SubclassOf+relation+ODP")


  






Retrieved from "[http://ontologydesignpatterns.org/wiki/Submissions:Lexico\_Syntactic\_ODP\_corresponding\_to\_SubclassOf\_relation\_ODP](../Submissions/Lexico_Syntactic_ODP_corresponding_to_SubclassOf_relation_ODP.md)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [ProposedLexicoSyntacticOP](../Category/ProposedLexicoSyntacticOP.md "Category:ProposedLexicoSyntacticOP")