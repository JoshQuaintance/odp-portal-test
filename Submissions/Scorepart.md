[![](../images/thumb/b/b5/Certified.png/70px-Certified.png)](../Image/Certified.png.md "Certified.png") __This pattern has been certified.__
Related submission, with evaluation history, can be found __here__





#  Graphical representation


__Diagram__
_(this article has no graphical representation)_



#  General description


  




#  Elements


_The __Scorepart__ Content OP locally defines the following ontology elements:_



[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif.md "Class") __Part__ (owl:Class) A part of a a score notation or a symbolic notation assigned to a specific instrument. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[Part](../Submissions/Scorepart/Part.md "Submissions:Scorepart/Part") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif.md "Class") __Section__ (owl:Class) A group of notes that share the same metric and clef. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[Section](../Submissions/Scorepart/Section.md "Submissions:Scorepart/Section") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif.md "Class") __Instrument__ (owl:Class) Any of various devices or contrivances that can be used to produce musical tones or sound. Any taxonomy can be used to subsume this concept. The default one is one extracted by Ivan Herman from the Musicbrainz instrument taxonomy, conforming to SKOS. This concept holds a seeAlso link towards this taxonomy. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[Instrument](../Submissions/Scorepart/Instrument.md "Submissions:Scorepart/Instrument") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif.md "Class") __Voice__ (owl:Class) One of several parts that can be performed within the same staff (e.g. alto and soprano). 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[Voice](../Submissions/Scorepart/Voice.md "Submissions:Scorepart/Voice") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif.md "Class") __HomogeneousFragment__ (owl:Class) A group of notes that share the same metric and clef. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[HomogeneousFragment](../Submissions/Scorepart/HomogeneousFragment.md "Submissions:Scorepart/HomogeneousFragment") page_
[![DatatypeProperty](../images/thumb/a/a5/DatatypeProperty.gif/20px-DatatypeProperty.gif)](../Image/DatatypeProperty.gif.md "DatatypeProperty") __hasMidiProgram__ (owl:DatatypeProperty) The instrument playing a specific part expressed by a MIDI program. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[hasMidiProgram](../Submissions/Scorepart/hasMidiProgram.md "Submissions:Scorepart/hasMidiProgram") page_
[![DatatypeProperty](../images/thumb/a/a5/DatatypeProperty.gif/20px-DatatypeProperty.gif)](../Image/DatatypeProperty.gif.md "DatatypeProperty") __hasStaff__ (owl:DatatypeProperty) The staff assigned to a specific instrument part in a music score. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[hasStaff](../Submissions/Scorepart/hasStaff.md "Submissions:Scorepart/hasStaff") page_
[![DatatypeProperty](../images/thumb/a/a5/DatatypeProperty.gif/20px-DatatypeProperty.gif)](../Image/DatatypeProperty.gif.md "DatatypeProperty") __hasClef__ (owl:DatatypeProperty) The clef that describes the hight of a note in a music score. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[hasClef](../Submissions/Scorepart/hasClef.md "Submissions:Scorepart/hasClef") page_
[![DatatypeProperty](../images/thumb/a/a5/DatatypeProperty.gif/20px-DatatypeProperty.gif)](../Image/DatatypeProperty.gif.md "DatatypeProperty") __hasTempo__ (owl:DatatypeProperty) The tempo of an homogeneous fragment, expressed in bpm (integer). 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[hasTempo](../Submissions/Scorepart/hasTempo.md "Submissions:Scorepart/hasTempo") page_
[![DatatypeProperty](../images/thumb/a/a5/DatatypeProperty.gif/20px-DatatypeProperty.gif)](../Image/DatatypeProperty.gif.md "DatatypeProperty") __hasMetric__ (owl:DatatypeProperty) The metric of a specific section of a music score. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[hasMetric](../Submissions/Scorepart/hasMetric.md "Submissions:Scorepart/hasMetric") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __isPlayedBy__ (owl:ObjectProperty) Connects the part of the score/symbolic notation to the instrument that is assigned to play such part. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[isPlayedBy](../Submissions/Scorepart/isPlayedBy.md "Submissions:Scorepart/isPlayedBy") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __hasVoice__ (owl:ObjectProperty) Connects the part of the score/symbolic notation to its constituing sections. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[hasVoice](../Submissions/Scorepart/hasVoice.md "Submissions:Scorepart/hasVoice") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __hasSection__ (owl:ObjectProperty) Connects the part of the score/symbolic notation to its constituing sections. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[hasSection](../Submissions/Scorepart/hasSection.md "Submissions:Scorepart/hasSection") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __hasFragment__ (owl:ObjectProperty) Connects the part of the score/symbolic notation to its constituing sections. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[hasFragment](../Submissions/Scorepart/hasFragment.md "Submissions:Scorepart/hasFragment") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __isFragmentOf__ (owl:ObjectProperty) Inverse of hasFragment 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[isFragmentOf](../Submissions/Scorepart/isFragmentOf.md "Submissions:Scorepart/isFragmentOf") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __isSectionOf__ (owl:ObjectProperty) Inverse of hasSection. Connects the section of the score/symbolic notation to the belongng part. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[isSectionOf](../Submissions/Scorepart/isSectionOf.md "Submissions:Scorepart/isSectionOf") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __isVoiceOf__ (owl:ObjectProperty) Inverse of hasVoice. Connects the voice of the score/symbolic notation to the belonging part. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[isVoiceOf](../Submissions/Scorepart/isVoiceOf.md "Submissions:Scorepart/isVoiceOf") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __playsPart__ (owl:ObjectProperty) Inverse of isPlayedBy. Connects an instrument to the the part that the instrument plays. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[playsPart](../Submissions/Scorepart/playsPart.md "Submissions:Scorepart/playsPart") page_
#  Additional information


#  Scenarios



__Scenarios about Scorepart__
No scenario is added to this Content OP.




#  Reviews



__Reviews about Scorepart__
There is no review about this proposal.
This revision (revision ID __14271__) takes in account the reviews: none


Other info at [evaluation tab](http://ontologydesignpatterns.org/wiki/index.php?title=Submissions:Scorepart&action=evaluation "http://ontologydesignpatterns.org/wiki/index.php?title=Submissions:Scorepart&action=evaluation")




#  Modeling issues



__Modeling issues about Scorepart__
There is no Modeling issue related to this proposal.




#  References


[Add a reference](index.php@title=Odp%253AAdd_reference&subject=../Submissions/Scorepart.md "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_reference&subject=Submissions%3AScorepart")


  

The Score Part pattern models the structure and the hierarchies of a music score.
In this module are used as template the following Ontology Design Patterns:





Retrieved from "[http://ontologydesignpatterns.org/wiki/Submissions:Scorepart](../Submissions/Scorepart.md)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [ProposedContentOP](../Category/ProposedContentOP.md "Category:ProposedContentOP")