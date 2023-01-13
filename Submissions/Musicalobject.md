[![](../images/thumb/b/b5/Certified.png/70px-Certified.png)](../Image/Certified.png.md "Certified.png") __This pattern has been certified.__
Related submission, with evaluation history, can be found __here__





#  Graphical representation


__Diagram__




[![Image:Musicalobject_pattern.png](../images/b/ba/Musicalobject_pattern.png)](../Image/Musicalobject_pattern.png.md "Image:Musicalobject_pattern.png")




#  General description


  




#  Elements


_The __Musicalobject__ Content OP locally defines the following ontology elements:_



[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif.md "Class") __Envelope__ (owl:Class) The envelope of a musical object's soundwave. In physics and engineering, the envelope of an oscillating signal is a smooth curve outlining its extremes. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[Envelope](../Submissions/Musicalobject/Envelope.md "Submissions:Musicalobject/Envelope") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif.md "Class") __Frequency__ (owl:Class) The frequency of a musical object. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[Frequency](../Submissions/Musicalobject/Frequency.md "Submissions:Musicalobject/Frequency") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif.md "Class") __FundamentalFrequency__ (owl:Class) The foundamental frequency of a musical object. The fundamental frequency is defined as the frequency of the lowest constituing partial of a signal. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[FundamentalFrequency](../Submissions/Musicalobject/FundamentalFrequency.md "Submissions:Musicalobject/FundamentalFrequency") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif.md "Class") __PartialFrequency__ (owl:Class) A frequency other than the foundamental Frequencyuency. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[PartialFrequency](../Submissions/Musicalobject/PartialFrequency.md "Submissions:Musicalobject/PartialFrequency") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif.md "Class") __MusicalObject__ (owl:Class) A musical object is the result of the realisation of a set of instructions that the musician or a computer system uses to realise a piece of music (e.g. music notation). 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[MusicalObject](../Submissions/Musicalobject/MusicalObject.md "Submissions:Musicalobject/MusicalObject") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif.md "Class") __MusicalObjectDuration__ (owl:Class) The duration of a musical object. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[MusicalObjectDuration](../Submissions/Musicalobject/MusicalObjectDuration.md "Submissions:Musicalobject/MusicalObjectDuration") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif.md "Class") __SoundIntensity__ (owl:Class) The intensity of the sound produced by a musical object. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[SoundIntensity](../Submissions/Musicalobject/SoundIntensity.md "Submissions:Musicalobject/SoundIntensity") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __hasDuration__ (owl:ObjectProperty) Connects a musical object to its duration. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[hasDuration](../Submissions/Musicalobject/hasDuration.md "Submissions:Musicalobject/hasDuration") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __hasEnvelope__ (owl:ObjectProperty) Connects a musical object to the envelope of the soundwave it produces. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[hasEnvelope](../Submissions/Musicalobject/hasEnvelope.md "Submissions:Musicalobject/hasEnvelope") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __hasFrequency__ (owl:ObjectProperty) Connects a musical object to the frequencies it produces. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[hasFrequency](../Submissions/Musicalobject/hasFrequency.md "Submissions:Musicalobject/hasFrequency") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __hasSoundIntensity__ (owl:ObjectProperty) Connects a musical object to the sound intensity produced. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[hasSoundIntensity](../Submissions/Musicalobject/hasSoundIntensity.md "Submissions:Musicalobject/hasSoundIntensity") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __isDurationOf__ (owl:ObjectProperty) Inverse of hasDuration. Connects the duration of a musical event to the musical event itself. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[isDurationOf](../Submissions/Musicalobject/isDurationOf.md "Submissions:Musicalobject/isDurationOf") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __isEnvelopeOf__ (owl:ObjectProperty) Inverse of hasEvelope. Connects the envelope of a musical event to the musical event itself. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[isEnvelopeOf](../Submissions/Musicalobject/isEnvelopeOf.md "Submissions:Musicalobject/isEnvelopeOf") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __isFrequencyOf__ (owl:ObjectProperty) Inverse of hasFrequency. Connects the frequency of a musical event to the musical event itself. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[isFrequencyOf](../Submissions/Musicalobject/isFrequencyOf.md "Submissions:Musicalobject/isFrequencyOf") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __isSoundIntensityOf__ (owl:ObjectProperty) Inverse of hasSoundIntensity. Connects the sound intensity of a musical event to the musical event itself. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[isSoundIntensityOf](../Submissions/Musicalobject/isSoundIntensityOf.md "Submissions:Musicalobject/isSoundIntensityOf") page_
[![DatatypeProperty](../images/thumb/a/a5/DatatypeProperty.gif/20px-DatatypeProperty.gif)](../Image/DatatypeProperty.gif.md "DatatypeProperty") __hasAttack__ (owl:DatatypeProperty) Describes the attack time (expressed in seconds) of the soundwave's envelope, according to the ADSR model. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[hasAttack](../Submissions/Musicalobject/hasAttack.md "Submissions:Musicalobject/hasAttack") page_
[![DatatypeProperty](../images/thumb/a/a5/DatatypeProperty.gif/20px-DatatypeProperty.gif)](../Image/DatatypeProperty.gif.md "DatatypeProperty") __hasDecay__ (owl:DatatypeProperty) Describes the decay time (epressed in seconds) of the soundwave's envelope, according to the ADSR model. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[hasDecay](../Submissions/Musicalobject/hasDecay.md "Submissions:Musicalobject/hasDecay") page_
[![DatatypeProperty](../images/thumb/a/a5/DatatypeProperty.gif/20px-DatatypeProperty.gif)](../Image/DatatypeProperty.gif.md "DatatypeProperty") __hasDurationInSeconds__ (owl:DatatypeProperty) Expresses the duration in seconds of a musical object. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[hasDurationInSeconds](../Submissions/Musicalobject/hasDurationInSeconds.md "Submissions:Musicalobject/hasDurationInSeconds") page_
[![DatatypeProperty](../images/thumb/a/a5/DatatypeProperty.gif/20px-DatatypeProperty.gif)](../Image/DatatypeProperty.gif.md "DatatypeProperty") __hasFrequencyMagnitude__ (owl:DatatypeProperty) The amplitude of a frequency component of a complex sound. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[hasFrequencyMagnitude](../Submissions/Musicalobject/hasFrequencyMagnitude.md "Submissions:Musicalobject/hasFrequencyMagnitude") page_
[![DatatypeProperty](../images/thumb/a/a5/DatatypeProperty.gif/20px-DatatypeProperty.gif)](../Image/DatatypeProperty.gif.md "DatatypeProperty") __hasIntensityValue__ (owl:DatatypeProperty) The value of the sound intensity of a musical object. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[hasIntensityValue](../Submissions/Musicalobject/hasIntensityValue.md "Submissions:Musicalobject/hasIntensityValue") page_
[![DatatypeProperty](../images/thumb/a/a5/DatatypeProperty.gif/20px-DatatypeProperty.gif)](../Image/DatatypeProperty.gif.md "DatatypeProperty") __hasRelease__ (owl:DatatypeProperty) Describes the release time (epressed in seconds) of the soundwave's envelope, according to the ADSR model. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[hasRelease](../Submissions/Musicalobject/hasRelease.md "Submissions:Musicalobject/hasRelease") page_
[![DatatypeProperty](../images/thumb/a/a5/DatatypeProperty.gif/20px-DatatypeProperty.gif)](../Image/DatatypeProperty.gif.md "DatatypeProperty") __hasSustain__ (owl:DatatypeProperty) Describes the sustain time (epressed in seconds) of the soundwave's envelope, according to the ADSR model. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[hasSustain](../Submissions/Musicalobject/hasSustain.md "Submissions:Musicalobject/hasSustain") page_
#  Additional information


#  Scenarios



__Scenarios about Musicalobject__
No scenario is added to this Content OP.




#  Reviews



__Reviews about Musicalobject__
There is no review about this proposal.
This revision (revision ID __14258__) takes in account the reviews: none


Other info at [evaluation tab](http://ontologydesignpatterns.org/wiki/index.php?title=Submissions:Musicalobject&action=evaluation "http://ontologydesignpatterns.org/wiki/index.php?title=Submissions:Musicalobject&action=evaluation")




  




#  Modeling issues



__Modeling issues about Musicalobject__
There is no Modeling issue related to this proposal.




  




#  References


[Add a reference](index.php@title=Odp%253AAdd_reference&subject=../Submissions/Musicalobject.md "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_reference&subject=Submissions%3AMusicalobject")


  






Retrieved from "[http://ontologydesignpatterns.org/wiki/Submissions:Musicalobject](../Submissions/Musicalobject.md)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [ProposedContentOP](../Category/ProposedContentOP.md "Category:ProposedContentOP")