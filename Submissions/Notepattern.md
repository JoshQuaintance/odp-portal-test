[![](../images/thumb/b/b5/Certified.png/70px-Certified.png)](../Image/Certified.png.md "Certified.png") __This pattern has been certified.__
Related submission, with evaluation history, can be found __here__





#  Graphical representation


__Diagram__




[![Image:Scorepart_pattern.png](../images/0/02/Scorepart_pattern.png)](../Image/Scorepart_pattern.png.md "Image:Scorepart_pattern.png")




#  General description


  




#  Elements


_The __Notepattern__ Content OP locally defines the following ontology elements:_



[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif.md "Class") __SymbolicNote__ (owl:Class) A music note from the western temperament system. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[SymbolicNote](../Submissions/Notepattern/SymbolicNote.md "Submissions:Notepattern/SymbolicNote") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif.md "Class") __Accidental__ (owl:Class) The accidental of a note (e.g. sharp). 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[Accidental](../Submissions/Notepattern/Accidental.md "Submissions:Notepattern/Accidental") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif.md "Class") __Position__ (owl:Class) The position of a symbolic note 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[Position](../Submissions/Notepattern/Position.md "Submissions:Notepattern/Position") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif.md "Class") __NotePitch__ (owl:Class) The pitch of a symbolic note. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[NotePitch](../Submissions/Notepattern/NotePitch.md "Submissions:Notepattern/NotePitch") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif.md "Class") __NoteDuration__ (owl:Class) The quantised duration of a symbolic music note. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[NoteDuration](../Submissions/Notepattern/NoteDuration.md "Submissions:Notepattern/NoteDuration") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif.md "Class") __NoteDynamic__ (owl:Class) The dynamic of a symbolic note. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[NoteDynamic](../Submissions/Notepattern/NoteDynamic.md "Submissions:Notepattern/NoteDynamic") page_
[![DatatypeProperty](../images/thumb/a/a5/DatatypeProperty.gif/20px-DatatypeProperty.gif)](../Image/DatatypeProperty.gif.md "DatatypeProperty") __hasMeasure__ (owl:DatatypeProperty) The measure (expressed in bars) to which a note belongs in a music score. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[hasMeasure](../Submissions/Notepattern/hasMeasure.md "Submissions:Notepattern/hasMeasure") page_
[![DatatypeProperty](../images/thumb/a/a5/DatatypeProperty.gif/20px-DatatypeProperty.gif)](../Image/DatatypeProperty.gif.md "DatatypeProperty") __hasMeasurePosition__ (owl:DatatypeProperty) The position the symbolic note have within the bar 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[hasMeasurePosition](../Submissions/Notepattern/hasMeasurePosition.md "Submissions:Notepattern/hasMeasurePosition") page_
[![DatatypeProperty](../images/thumb/a/a5/DatatypeProperty.gif/20px-DatatypeProperty.gif)](../Image/DatatypeProperty.gif.md "DatatypeProperty") __hasMidiPitch__ (owl:DatatypeProperty) The pitch of a note expressed by means of its MIDI number. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[hasMidiPitch](../Submissions/Notepattern/hasMidiPitch.md "Submissions:Notepattern/hasMidiPitch") page_
[![DatatypeProperty](../images/thumb/a/a5/DatatypeProperty.gif/20px-DatatypeProperty.gif)](../Image/DatatypeProperty.gif.md "DatatypeProperty") __isDefinedByOctave__ (owl:DatatypeProperty) The octave on which the note is defined. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[isDefinedByOctave](../Submissions/Notepattern/isDefinedByOctave.md "Submissions:Notepattern/isDefinedByOctave") page_
[![DatatypeProperty](../images/thumb/a/a5/DatatypeProperty.gif/20px-DatatypeProperty.gif)](../Image/DatatypeProperty.gif.md "DatatypeProperty") __hasLiteralDynamic__ (owl:DatatypeProperty) The dynamic expressed in a music score by means of adjectives (e.g. piano). 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[hasLiteralDynamic](../Submissions/Notepattern/hasLiteralDynamic.md "Submissions:Notepattern/hasLiteralDynamic") page_
[![DatatypeProperty](../images/thumb/a/a5/DatatypeProperty.gif/20px-DatatypeProperty.gif)](../Image/DatatypeProperty.gif.md "DatatypeProperty") __hasMidiVelocity__ (owl:DatatypeProperty) The dynamics of the note expressed symbolically by means of the MIDI command "velocity". 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[hasMidiVelocity](../Submissions/Notepattern/hasMidiVelocity.md "Submissions:Notepattern/hasMidiVelocity") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __hasNoteDynamic__ (owl:ObjectProperty) Connects a symbolic note to its symbolic dynamic. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[hasNoteDynamic](../Submissions/Notepattern/hasNoteDynamic.md "Submissions:Notepattern/hasNoteDynamic") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __isDynamicOf__ (owl:ObjectProperty) Inverse of hasNoteDynamic. Connects a duration class to the symbolic note that have this specific dynamic. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[isDynamicOf](../Submissions/Notepattern/isDynamicOf.md "Submissions:Notepattern/isDynamicOf") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __hasNoteDuration__ (owl:ObjectProperty) Connects a symbolic note to its symbolic quantised duration. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[hasNoteDuration](../Submissions/Notepattern/hasNoteDuration.md "Submissions:Notepattern/hasNoteDuration") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __isDurationOfNote__ (owl:ObjectProperty) Inverse of hasNoteDuration. Connects a duration class to the symbolic note that have this specific duration. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[isDurationOfNote](../Submissions/Notepattern/isDurationOfNote.md "Submissions:Notepattern/isDurationOfNote") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __hasNotePitch__ (owl:ObjectProperty) Connects a symbolic note to its symbolic pitch. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[hasNotePitch](../Submissions/Notepattern/hasNotePitch.md "Submissions:Notepattern/hasNotePitch") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __isPitchOf__ (owl:ObjectProperty) Inverse of hasPitch. Connects a duration class to the symbolic note that have this specific pitch. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[isPitchOf](../Submissions/Notepattern/isPitchOf.md "Submissions:Notepattern/isPitchOf") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __hasAccidental__ (owl:ObjectProperty) The accidental of a note (e.g. sharp). 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[hasAccidental](../Submissions/Notepattern/hasAccidental.md "Submissions:Notepattern/hasAccidental") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __isAccidentalOf__ (owl:ObjectProperty) Inverse of hasAccidental 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[isAccidentalOf](../Submissions/Notepattern/isAccidentalOf.md "Submissions:Notepattern/isAccidentalOf") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __hasPosition__ (owl:ObjectProperty) Connects the symbolic note with its duration 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[hasPosition](../Submissions/Notepattern/hasPosition.md "Submissions:Notepattern/hasPosition") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __isPositionOf__ (owl:ObjectProperty) Inverse of hasPosition 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[isPositionOf](../Submissions/Notepattern/isPositionOf.md "Submissions:Notepattern/isPositionOf") page_
  




#  Additional information


#  Scenarios



__Scenarios about Notepattern__
No scenario is added to this Content OP.




#  Reviews



__Reviews about Notepattern__
There is no review about this proposal.
This revision (revision ID __14262__) takes in account the reviews: none


Other info at [evaluation tab](http://ontologydesignpatterns.org/wiki/index.php?title=Submissions:Notepattern&action=evaluation "http://ontologydesignpatterns.org/wiki/index.php?title=Submissions:Notepattern&action=evaluation")




#  Modeling issues



__Modeling issues about Notepattern__
There is no Modeling issue related to this proposal.




#  References


[Add a reference](index.php@title=Odp%253AAdd_reference&subject=../Submissions/Notepattern.md "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_reference&subject=Submissions%3ANotepattern")


  

The Note Pattern models a music note both in relation to a music score and in relation to the musical object produced by playing such note.





Retrieved from "[http://ontologydesignpatterns.org/wiki/Submissions:Notepattern](../Submissions/Notepattern.md)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [ProposedContentOP](../Category/ProposedContentOP.md "Category:ProposedContentOP")