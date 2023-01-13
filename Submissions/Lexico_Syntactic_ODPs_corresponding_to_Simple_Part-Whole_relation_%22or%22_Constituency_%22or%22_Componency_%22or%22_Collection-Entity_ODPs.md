[![](../images/thumb/b/b5/Certified.png/70px-Certified.png)](../Image/Certified.png "Certified.png") __This pattern has been certified.__
Related submission, with evaluation history, can be found __here__





#  Description


  




#  Cases


_The __Lexico Syntactic ODPs corresponding to Simple Part-Whole relation "or" Constituency "or" Componency "or" Collection-Entity ODPs__ Lexico-Syntactic ODP includes the following cases (see also [abbreviations and symbols used in LSP Formalization](../Community/LSPSymbols "Community:LSPSymbols")):_


  






__NL Formulation__



* Proteins form part of the cell membrane.


__LSP Formalization__




```
[(NP<part>,)* and] NP<part> PART NP<whole>

```

__Reusable JAPE code__: [PW\_1.jape](../images/d/db/PW_1.jape "PW 1.jape")





[![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[1](Submissions%253ALexico_Syntactic_ODPs_corresponding_to_Simple_Part-Whole_relation_%2522or%2522_Constituency_%2522or%2522_Componency_%2522or%2522_Collection-Entity_ODPs/1.html "Submissions:Lexico Syntactic ODPs corresponding to Simple Part-Whole relation \"or\" Constituency \"or\" Componency \"or\" Collection-Entity ODPs/1") page_





__NL Formulation__



* Most clays consist of flat particles.
* Water is made up of hydrogen and oxygen.
* The United Arab Emirates is a country composed of seven emirates or sheikdoms.


__LSP Formalization__




```
NP<whole> PART [(NP<part>,)* and] NP<part>

```

__Reusable JAPE code__: [PW\_2.jape](../images/8/89/PW_2.jape "PW 2.jape")





[![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[2](Submissions%253ALexico_Syntactic_ODPs_corresponding_to_Simple_Part-Whole_relation_%2522or%2522_Constituency_%2522or%2522_Componency_%2522or%2522_Collection-Entity_ODPs/2.html "Submissions:Lexico Syntactic ODPs corresponding to Simple Part-Whole relation \"or\" Constituency \"or\" Componency \"or\" Collection-Entity ODPs/2") page_





__NL Formulation__



* A state machine workflow is made up of a set of states, transitions, and actions.


__LSP Formalization__




```
NP<whole> be PART [CD] CN-PART [PARA] [(NP<part>,)* and] NP<part>

```

__Reusable JAPE code__: -





[![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[3](Submissions%253ALexico_Syntactic_ODPs_corresponding_to_Simple_Part-Whole_relation_%2522or%2522_Constituency_%2522or%2522_Componency_%2522or%2522_Collection-Entity_ODPs/3.html "Submissions:Lexico Syntactic ODPs corresponding to Simple Part-Whole relation \"or\" Constituency \"or\" Componency \"or\" Collection-Entity ODPs/3") page_





__NL Formulation__



* The parts of a tree are the root, trunk(s), branches, twigs and leaves.


__LSP Formalization__




```
CN-PART  NP<whole> be [PARA] [(NP<part>,)* and] NP<part>

```

__Reusable JAPE code__: [PW\_3.jape](../images/4/48/PW_3.jape "PW 3.jape")





[![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[4](Submissions%253ALexico_Syntactic_ODPs_corresponding_to_Simple_Part-Whole_relation_%2522or%2522_Constituency_%2522or%2522_Componency_%2522or%2522_Collection-Entity_ODPs/4.html "Submissions:Lexico Syntactic ODPs corresponding to Simple Part-Whole relation \"or\" Constituency \"or\" Componency \"or\" Collection-Entity ODPs/4") page_





__NL Formulation__



* The cerebrum is divided into two major parts: the right cerebral hemisphere and left cerebral hemisphere.


__LSP Formalization__




```
NP<whole> include/(be divide in/into)/(be separate in/into)CD CN-PART [PARA] [(NP<part>,)* and] NP<part

```

__Reusable JAPE code__: [PW\_5.jape](../images/7/7a/PW_5.jape "PW 5.jape")





[![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[5](Submissions%253ALexico_Syntactic_ODPs_corresponding_to_Simple_Part-Whole_relation_%2522or%2522_Constituency_%2522or%2522_Componency_%2522or%2522_Collection-Entity_ODPs/5.html "Submissions:Lexico Syntactic ODPs corresponding to Simple Part-Whole relation \"or\" Constituency \"or\" Componency \"or\" Collection-Entity ODPs/5") page_



#  Additional information


#  Reviews



__Reviews about Lexico Syntactic ODPs corresponding to Simple Part-Whole relation "or" Constituency "or" Componency "or" Collection-Entity ODPs__
There is no review about this proposal.
This revision (revision ID __8984__) takes in account the reviews: none


Other info at [evaluation tab](http://ontologydesignpatterns.org/wiki/index.php?title=Submissions:Lexico_Syntactic_ODPs_corresponding_to_Simple_Part-Whole_relation_%22or%22_Constituency_%22or%22_Componency_%22or%22_Collection-Entity_ODPs&action=evaluation "http://ontologydesignpatterns.org/wiki/index.php?title=Submissions:Lexico_Syntactic_ODPs_corresponding_to_Simple_Part-Whole_relation_%22or%22_Constituency_%22or%22_Componency_%22or%22_Collection-Entity_ODPs&action=evaluation")




  




#  Modeling issues



__Modeling issues about Lexico Syntactic ODPs corresponding to Simple Part-Whole relation "or" Constituency "or" Componency "or" Collection-Entity ODPs__
There is no Modeling issue related to this proposal.




  




#  References


[Add a reference](index.php@title=Odp%253AAdd_reference&subject=Submissions%253ALexico+Syntactic+ODPs+corresponding+to+Simple+Part-Whole+relation+&quot%3Bor&quot%3B+Constituency+&quot%3Bor&quot%3B+Componency+&quot%3Bor&quot%3B+Collection-Entity+ODPs.html "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_reference&subject=Submissions%3ALexico+Syntactic+ODPs+corresponding+to+Simple+Part-Whole+relation+%26quot%3Bor%26quot%3B+Constituency+%26quot%3Bor%26quot%3B+Componency+%26quot%3Bor%26quot%3B+Collection-Entity+ODPs")


  






Retrieved from "[http://ontologydesignpatterns.org/wiki/Submissions:Lexico\_Syntactic\_ODPs\_corresponding\_to\_Simple\_Part-Whole\_relation\_%22or%22\_Constituency\_%22or%22\_Componency\_%22or%22\_Collection-Entity\_ODPs](Submissions%253ALexico_Syntactic_ODPs_corresponding_to_Simple_Part-Whole_relation_%2522or%2522_Constituency_%2522or%2522_Componency_%2522or%2522_Collection-Entity_ODPs.html)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [ProposedLexicoSyntacticOP](../Category/ProposedLexicoSyntacticOP "Category:ProposedLexicoSyntacticOP")