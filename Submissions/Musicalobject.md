[![](../images/thumb/b/b5/Certified.png/70px-Certified.png)](../Image/Certified.png "Certified.png") __This pattern has been certified.__
Related submission, with evaluation history, can be found __here__





#  Graphical representation


__Diagram__




[![Image:Musicalobject_pattern.png](../images/b/ba/Musicalobject_pattern.png)](../Image/Musicalobject_pattern.png "Image:Musicalobject_pattern.png")




#  General description


  




#  Elements


_The __Musicalobject__ Content OP locally defines the following ontology elements:_



[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif "Class") __Envelope__ (owl:Class) The envelope of a musical object's soundwave. In physics and engineering, the envelope of an oscillating signal is a smooth curve outlining its extremes. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[Envelope](../Submissions/Musicalobject/Envelope "Submissions:Musicalobject/Envelope") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif "Class") __Frequency__ (owl:Class) The frequency of a musical object. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[Frequency](../Submissions/Musicalobject/Frequency "Submissions:Musicalobject/Frequency") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif "Class") __FundamentalFrequency__ (owl:Class) The foundamental frequency of a musical object. The fundamental frequency is defined as the frequency of the lowest constituing partial of a signal. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[FundamentalFrequency](../Submissions/Musicalobject/FundamentalFrequency "Submissions:Musicalobject/FundamentalFrequency") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif "Class") __PartialFrequency__ (owl:Class) A frequency other than the foundamental Frequencyuency. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[PartialFrequency](../Submissions/Musicalobject/PartialFrequency "Submissions:Musicalobject/PartialFrequency") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif "Class") __MusicalObject__ (owl:Class) A musical object is the result of the realisation of a set of instructions that the musician or a computer system uses to realise a piece of music (e.g. music notation). 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[MusicalObject](../Submissions/Musicalobject/MusicalObject "Submissions:Musicalobject/MusicalObject") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif "Class") __MusicalObjectDuration__ (owl:Class) The duration of a musical object. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[MusicalObjectDuration](../Submissions/Musicalobject/MusicalObjectDuration "Submissions:Musicalobject/MusicalObjectDuration") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif "Class") __SoundIntensity__ (owl:Class) The intensity of the sound produced by a musical object. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[SoundIntensity](../Submissions/Musicalobject/SoundIntensity "Submissions:Musicalobject/SoundIntensity") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif "ObjectProperty") __hasDuration__ (owl:ObjectProperty) Connects a musical object to its duration. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[hasDuration](../Submissions/Musicalobject/hasDuration "Submissions:Musicalobject/hasDuration") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif "ObjectProperty") __hasEnvelope__ (owl:ObjectProperty) Connects a musical object to the envelope of the soundwave it produces. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[hasEnvelope](../Submissions/Musicalobject/hasEnvelope "Submissions:Musicalobject/hasEnvelope") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif "ObjectProperty") __hasFrequency__ (owl:ObjectProperty) Connects a musical object to the frequencies it produces. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[hasFrequency](../Submissions/Musicalobject/hasFrequency "Submissions:Musicalobject/hasFrequency") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif "ObjectProperty") __hasSoundIntensity__ (owl:ObjectProperty) Connects a musical object to the sound intensity produced. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[hasSoundIntensity](../Submissions/Musicalobject/hasSoundIntensity "Submissions:Musicalobject/hasSoundIntensity") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif "ObjectProperty") __isDurationOf__ (owl:ObjectProperty) Inverse of hasDuration. Connects the duration of a musical event to the musical event itself. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[isDurationOf](../Submissions/Musicalobject/isDurationOf "Submissions:Musicalobject/isDurationOf") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif "ObjectProperty") __isEnvelopeOf__ (owl:ObjectProperty) Inverse of hasEvelope. Connects the envelope of a musical event to the musical event itself. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[isEnvelopeOf](../Submissions/Musicalobject/isEnvelopeOf "Submissions:Musicalobject/isEnvelopeOf") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif "ObjectProperty") __isFrequencyOf__ (owl:ObjectProperty) Inverse of hasFrequency. Connects the frequency of a musical event to the musical event itself. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[isFrequencyOf](../Submissions/Musicalobject/isFrequencyOf "Submissions:Musicalobject/isFrequencyOf") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif "ObjectProperty") __isSoundIntensityOf__ (owl:ObjectProperty) Inverse of hasSoundIntensity. Connects the sound intensity of a musical event to the musical event itself. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[isSoundIntensityOf](../Submissions/Musicalobject/isSoundIntensityOf "Submissions:Musicalobject/isSoundIntensityOf") page_
[![DatatypeProperty](../images/thumb/a/a5/DatatypeProperty.gif/20px-DatatypeProperty.gif)](../Image/DatatypeProperty.gif "DatatypeProperty") __hasAttack__ (owl:DatatypeProperty) Describes the attack time (expressed in seconds) of the soundwave's envelope, according to the ADSR model. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[hasAttack](../Submissions/Musicalobject/hasAttack "Submissions:Musicalobject/hasAttack") page_
[![DatatypeProperty](../images/thumb/a/a5/DatatypeProperty.gif/20px-DatatypeProperty.gif)](../Image/DatatypeProperty.gif "DatatypeProperty") __hasDecay__ (owl:DatatypeProperty) Describes the decay time (epressed in seconds) of the soundwave's envelope, according to the ADSR model. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[hasDecay](../Submissions/Musicalobject/hasDecay "Submissions:Musicalobject/hasDecay") page_
[![DatatypeProperty](../images/thumb/a/a5/DatatypeProperty.gif/20px-DatatypeProperty.gif)](../Image/DatatypeProperty.gif "DatatypeProperty") __hasDurationInSeconds__ (owl:DatatypeProperty) Expresses the duration in seconds of a musical object. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[hasDurationInSeconds](../Submissions/Musicalobject/hasDurationInSeconds "Submissions:Musicalobject/hasDurationInSeconds") page_
[![DatatypeProperty](../images/thumb/a/a5/DatatypeProperty.gif/20px-DatatypeProperty.gif)](../Image/DatatypeProperty.gif "DatatypeProperty") __hasFrequencyMagnitude__ (owl:DatatypeProperty) The amplitude of a frequency component of a complex sound. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[hasFrequencyMagnitude](../Submissions/Musicalobject/hasFrequencyMagnitude "Submissions:Musicalobject/hasFrequencyMagnitude") page_
[![DatatypeProperty](../images/thumb/a/a5/DatatypeProperty.gif/20px-DatatypeProperty.gif)](../Image/DatatypeProperty.gif "DatatypeProperty") __hasIntensityValue__ (owl:DatatypeProperty) The value of the sound intensity of a musical object. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[hasIntensityValue](../Submissions/Musicalobject/hasIntensityValue "Submissions:Musicalobject/hasIntensityValue") page_
[![DatatypeProperty](../images/thumb/a/a5/DatatypeProperty.gif/20px-DatatypeProperty.gif)](../Image/DatatypeProperty.gif "DatatypeProperty") __hasRelease__ (owl:DatatypeProperty) Describes the release time (epressed in seconds) of the soundwave's envelope, according to the ADSR model. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[hasRelease](../Submissions/Musicalobject/hasRelease "Submissions:Musicalobject/hasRelease") page_
[![DatatypeProperty](../images/thumb/a/a5/DatatypeProperty.gif/20px-DatatypeProperty.gif)](../Image/DatatypeProperty.gif "DatatypeProperty") __hasSustain__ (owl:DatatypeProperty) Describes the sustain time (epressed in seconds) of the soundwave's envelope, according to the ADSR model. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[hasSustain](../Submissions/Musicalobject/hasSustain "Submissions:Musicalobject/hasSustain") page_
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


[Add a reference](index.php@title=Odp%253AAdd_reference&subject=../Submissions/Musicalobject "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_reference&subject=Submissions%3AMusicalobject")


  






Retrieved from "[http://ontologydesignpatterns.org/wiki/Submissions:Musicalobject](../Submissions/Musicalobject)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [ProposedContentOP](../Category/ProposedContentOP "Category:ProposedContentOP")