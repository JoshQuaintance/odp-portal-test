[![](../images/thumb/b/b5/Certified.png/70px-Certified.png)](../Image/Certified.png.md "Certified.png") __This pattern has been certified.__
Related submission, with evaluation history, can be found __here__





#  Graphical representation


__Diagram__




[![Image:CommunicationEvent.jpg](../images/a/aa/CommunicationEvent.jpg)](../Image/CommunicationEvent.jpg.md "Image:CommunicationEvent.jpg")




#  General description


  




#  Elements


_The __CommunicationEvent__ Content OP locally defines the following ontology elements:_



[![Class](../../../../../../../../../../../../../../../../../../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif.md "Class") __ContactMechanism__ (owl:Class) The medium for the communication. 
 [![](../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[ContactMechanism](../Submissions/CommunicationEvent/ContactMechanism.md "Submissions:CommunicationEvent/ContactMechanism") page_
[![ObjectProperty](../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __isValidContactMechanismFor__ (owl:ObjectProperty) 
 [![](../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[isValidContactMechanismFor](../Submissions/CommunicationEvent/isValidContactMechanismFor.md "Submissions:CommunicationEvent/isValidContactMechanismFor") page_
[![Class](../../../../../../../../../../../../../../../../../../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif.md "Class") __CommunicationEventRole__ (owl:Class) The role that this event plays for a specific party, e.g. a conference has the role of transmitting research results for a presenter while it has the role of generating income and connections for the organizers, and generating knowledge for the participants. 
 [![](../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[CommunicationEventRole](../Submissions/CommunicationEvent/CommunicationEventRole.md "Submissions:CommunicationEvent/CommunicationEventRole") page_
[![ObjectProperty](../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __mediumOf__ (owl:ObjectProperty) 
 [![](../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[mediumOf](../Submissions/CommunicationEvent/mediumOf.md "Submissions:CommunicationEvent/mediumOf") page_
[![Class](../../../../../../../../../../../../../../../../../../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif.md "Class") __CommunicationEvent__ (owl:Class) An instance of communication, e.g. a phone call, a meeting or a conference. 
 [![](../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[CommunicationEvent](../Submissions/CommunicationEvent/CommunicationEvent.md "Submissions:CommunicationEvent/CommunicationEvent") page_
[![Class](../../../../../../../../../../../../../../../../../../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif.md "Class") __EventDuration__ (owl:Class) The time duration of a communication event. 
 [![](../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[EventDuration](../Submissions/CommunicationEvent/EventDuration.md "Submissions:CommunicationEvent/EventDuration") page_
[![DatatypeProperty](../../../../images/thumb/a/a5/DatatypeProperty.gif/20px-DatatypeProperty.gif)](../Image/DatatypeProperty.gif.md "DatatypeProperty") __eventStartTime__ (owl:DatatypeProperty) 
 [![](../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[eventStartTime](../Submissions/CommunicationEvent/eventStartTime.md "Submissions:CommunicationEvent/eventStartTime") page_
[![Class](../../../../../../../../../../../../../../../../../../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif.md "Class") __RelationshipDuration__ (owl:Class) The time duration of a relationship. 
 [![](../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[RelationshipDuration](../Submissions/CommunicationEvent/RelationshipDuration.md "Submissions:CommunicationEvent/RelationshipDuration") page_
[![DatatypeProperty](../../../../images/thumb/a/a5/DatatypeProperty.gif/20px-DatatypeProperty.gif)](../Image/DatatypeProperty.gif.md "DatatypeProperty") __relationshipStartTime__ (owl:DatatypeProperty) 
 [![](../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[relationshipStartTime](../Submissions/CommunicationEvent/relationshipStartTime.md "Submissions:CommunicationEvent/relationshipStartTime") page_
[![Class](../../../../../../../../../../../../../../../../../../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif.md "Class") __PartyRole__ (owl:Class) The role of a party in a relationship, e.g. in a sales relationship one party has the customer role and the other party the provider role. 
 [![](../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[PartyRole](../Submissions/CommunicationEvent/PartyRole.md "Submissions:CommunicationEvent/PartyRole") page_
[![Class](../../../../../../../../../../../../../../../../../../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif.md "Class") __RelationshipPartyRole__ (owl:Class) The role of a specific party in a relationship, e.g. in this particular buyer-seller relationship company x is the seller. 
 [![](../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[RelationshipPartyRole](../Submissions/CommunicationEvent/RelationshipPartyRole.md "Submissions:CommunicationEvent/RelationshipPartyRole") page_
[![ObjectProperty](../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __roleInRelationship__ (owl:ObjectProperty) 
 [![](../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[roleInRelationship](../Submissions/CommunicationEvent/roleInRelationship.md "Submissions:CommunicationEvent/roleInRelationship") page_
[![Class](../../../../../../../../../../../../../../../../../../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif.md "Class") __PartyRelationship__ (owl:Class) An event in the sense of a state of things, where two or more parties are involved through different roles, e.g. a buyer-seller relation. 
 [![](../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[PartyRelationship](../Submissions/CommunicationEvent/PartyRelationship.md "Submissions:CommunicationEvent/PartyRelationship") page_
[![ObjectProperty](../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __includesCommunication__ (owl:ObjectProperty) 
 [![](../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[includesCommunication](../Submissions/CommunicationEvent/includesCommunication.md "Submissions:CommunicationEvent/includesCommunication") page_
[![ObjectProperty](../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __relationshipIncludes__ (owl:ObjectProperty) 
 [![](../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[relationshipIncludes](../Submissions/CommunicationEvent/relationshipIncludes.md "Submissions:CommunicationEvent/relationshipIncludes") page_
[![ObjectProperty](../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __relationshipHasDuration__ (owl:ObjectProperty) 
 [![](../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[relationshipHasDuration](../Submissions/CommunicationEvent/relationshipHasDuration.md "Submissions:CommunicationEvent/relationshipHasDuration") page_
[![Class](../../../../../../../../../../../../../../../../../../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif.md "Class") __EmailCommunication__ (owl:Class) 
 [![](../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[EmailCommunication](../Submissions/CommunicationEvent/EmailCommunication.md "Submissions:CommunicationEvent/EmailCommunication") page_
[![ObjectProperty](../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __throughMedium__ (owl:ObjectProperty) 
 [![](../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[throughMedium](../Submissions/CommunicationEvent/throughMedium.md "Submissions:CommunicationEvent/throughMedium") page_
__e-mail__ ([http://www.ontology.se/odp/content/owl/CommunicationEvent#ContactMechanism](http://www.ontology.se/odp/content/owl/CommunicationEvent#ContactMechanism "http://www.ontology.se/odp/content/owl/CommunicationEvent#ContactMechanism")) 
 [![](../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[e-mail](../Submissions/CommunicationEvent/e-mail.md "Submissions:CommunicationEvent/e-mail") page_
[![Class](../../../../../../../../../../../../../../../../../../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif.md "Class") __PhoneCommunication__ (owl:Class) 
 [![](../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[PhoneCommunication](../Submissions/CommunicationEvent/PhoneCommunication.md "Submissions:CommunicationEvent/PhoneCommunication") page_
__phone__ ([http://www.ontology.se/odp/content/owl/CommunicationEvent#ContactMechanism](http://www.ontology.se/odp/content/owl/CommunicationEvent#ContactMechanism "http://www.ontology.se/odp/content/owl/CommunicationEvent#ContactMechanism")) 
 [![](../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[phone](../Submissions/CommunicationEvent/phone.md "Submissions:CommunicationEvent/phone") page_
[![Class](../../../../../../../../../../../../../../../../../../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif.md "Class") __CommunicationPurpose__ (owl:Class) The purpose or goal of the communciation event. 
 [![](../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[CommunicationPurpose](../Submissions/CommunicationEvent/CommunicationPurpose.md "Submissions:CommunicationEvent/CommunicationPurpose") page_
[![ObjectProperty](../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __purposeOfEvent__ (owl:ObjectProperty) 
 [![](../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[purposeOfEvent](../Submissions/CommunicationEvent/purposeOfEvent.md "Submissions:CommunicationEvent/purposeOfEvent") page_
[![Class](../../../../../../../../../../../../../../../../../../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif.md "Class") __WebSiteCommunication__ (owl:Class) 
 [![](../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[WebSiteCommunication](../Submissions/CommunicationEvent/WebSiteCommunication.md "Submissions:CommunicationEvent/WebSiteCommunication") page_
__web-site__ ([http://www.ontology.se/odp/content/owl/CommunicationEvent#ContactMechanism](http://www.ontology.se/odp/content/owl/CommunicationEvent#ContactMechanism "http://www.ontology.se/odp/content/owl/CommunicationEvent#ContactMechanism")) 
 [![](../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[web-site](../Submissions/CommunicationEvent/web-site.md "Submissions:CommunicationEvent/web-site") page_
[![Class](../../../../../../../../../../../../../../../../../../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif.md "Class") __FaceToFaceCommunication__ (owl:Class) 
 [![](../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[FaceToFaceCommunication](../Submissions/CommunicationEvent/FaceToFaceCommunication.md "Submissions:CommunicationEvent/FaceToFaceCommunication") page_
__face-to-face__ ([http://www.ontology.se/odp/content/owl/CommunicationEvent#ContactMechanism](http://www.ontology.se/odp/content/owl/CommunicationEvent#ContactMechanism "http://www.ontology.se/odp/content/owl/CommunicationEvent#ContactMechanism")) 
 [![](../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[face-to-face](../Submissions/CommunicationEvent/face-to-face.md "Submissions:CommunicationEvent/face-to-face") page_
[![ObjectProperty](../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __roleOfParty__ (owl:ObjectProperty) 
 [![](../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[roleOfParty](../Submissions/CommunicationEvent/roleOfParty.md "Submissions:CommunicationEvent/roleOfParty") page_
[![ObjectProperty](../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __partyParticipating__ (owl:ObjectProperty) 
 [![](../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[partyParticipating](../Submissions/CommunicationEvent/partyParticipating.md "Submissions:CommunicationEvent/partyParticipating") page_
[![ObjectProperty](../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __inRelationship__ (owl:ObjectProperty) 
 [![](../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[inRelationship](../Submissions/CommunicationEvent/inRelationship.md "Submissions:CommunicationEvent/inRelationship") page_
[![Class](../../../../../../../../../../../../../../../../../../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif.md "Class") __Party__ (owl:Class) A physical or juridical party, e.g. person or organization. 
 [![](../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[Party](../Submissions/CommunicationEvent/Party.md "Submissions:CommunicationEvent/Party") page_
[![ObjectProperty](../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __partyInvolvedIn__ (owl:ObjectProperty) 
 [![](../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[partyInvolvedIn](../Submissions/CommunicationEvent/partyInvolvedIn.md "Submissions:CommunicationEvent/partyInvolvedIn") page_
[![Class](../../../../../../../../../../../../../../../../../../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif.md "Class") __CommunicationEventPartyRole__ (owl:Class) The role of a specific party for a specific communciation event, e.g. in this particular meeting John is the chairman. 
 [![](../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[CommunicationEventPartyRole](../Submissions/CommunicationEvent/CommunicationEventPartyRole.md "Submissions:CommunicationEvent/CommunicationEventPartyRole") page_
[![ObjectProperty](../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __partyInRelationship__ (owl:ObjectProperty) 
 [![](../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[partyInRelationship](../Submissions/CommunicationEvent/partyInRelationship.md "Submissions:CommunicationEvent/partyInRelationship") page_
[![ObjectProperty](../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __hasValidContactMechanism__ (owl:ObjectProperty) Relates roles of communication events to their valid mediums, e.g. it may only be allowed to send contracts by letter or fax but not e-mail. 
 [![](../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[hasValidContactMechanism](../Submissions/CommunicationEvent/hasValidContactMechanism.md "Submissions:CommunicationEvent/hasValidContactMechanism") page_
[![ObjectProperty](../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __eventRoleIncludedIn__ (owl:ObjectProperty) 
 [![](../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[eventRoleIncludedIn](../Submissions/CommunicationEvent/eventRoleIncludedIn.md "Submissions:CommunicationEvent/eventRoleIncludedIn") page_
[![Class](../../../../../../../../../../../../../../../../../../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif.md "Class") __LetterCorrespondence__ (owl:Class) 
 [![](../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[LetterCorrespondence](../Submissions/CommunicationEvent/LetterCorrespondence.md "Submissions:CommunicationEvent/LetterCorrespondence") page_
__letter__ ([http://www.ontology.se/odp/content/owl/CommunicationEvent#ContactMechanism](http://www.ontology.se/odp/content/owl/CommunicationEvent#ContactMechanism "http://www.ontology.se/odp/content/owl/CommunicationEvent#ContactMechanism")) 
 [![](../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[letter](../Submissions/CommunicationEvent/letter.md "Submissions:CommunicationEvent/letter") page_
[![Class](../../../../../../../../../../../../../../../../../../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif.md "Class") __FaxCommunication__ (owl:Class) 
 [![](../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[FaxCommunication](../Submissions/CommunicationEvent/FaxCommunication.md "Submissions:CommunicationEvent/FaxCommunication") page_
__fax__ ([http://www.ontology.se/odp/content/owl/CommunicationEvent#ContactMechanism](http://www.ontology.se/odp/content/owl/CommunicationEvent#ContactMechanism "http://www.ontology.se/odp/content/owl/CommunicationEvent#ContactMechanism")) 
 [![](../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[fax](../Submissions/CommunicationEvent/fax.md "Submissions:CommunicationEvent/fax") page_
[![ObjectProperty](../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __roleOfEvent__ (owl:ObjectProperty) 
 [![](../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[roleOfEvent](../Submissions/CommunicationEvent/roleOfEvent.md "Submissions:CommunicationEvent/roleOfEvent") page_
[![ObjectProperty](../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __partyInEvent__ (owl:ObjectProperty) 
 [![](../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[partyInEvent](../Submissions/CommunicationEvent/partyInEvent.md "Submissions:CommunicationEvent/partyInEvent") page_
[![ObjectProperty](../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __inCommunicationEvent__ (owl:ObjectProperty) 
 [![](../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[inCommunicationEvent](../Submissions/CommunicationEvent/inCommunicationEvent.md "Submissions:CommunicationEvent/inCommunicationEvent") page_
[![ObjectProperty](../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __eventIncludes__ (owl:ObjectProperty) 
 [![](../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[eventIncludes](../Submissions/CommunicationEvent/eventIncludes.md "Submissions:CommunicationEvent/eventIncludes") page_
[![ObjectProperty](../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __communicationHasSetting__ (owl:ObjectProperty) All communications take place within some relationship between parties, e.g. a sales call takes place within the relationship with a prospective customer. 
 [![](../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[communicationHasSetting](../Submissions/CommunicationEvent/communicationHasSetting.md "Submissions:CommunicationEvent/communicationHasSetting") page_
[![ObjectProperty](../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __eventHasPurpose__ (owl:ObjectProperty) 
 [![](../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[eventHasPurpose](../Submissions/CommunicationEvent/eventHasPurpose.md "Submissions:CommunicationEvent/eventHasPurpose") page_
[![ObjectProperty](../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __eventHasDuration__ (owl:ObjectProperty) 
 [![](../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[eventHasDuration](../Submissions/CommunicationEvent/eventHasDuration.md "Submissions:CommunicationEvent/eventHasDuration") page_
[![ObjectProperty](../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __hasEventStatus__ (owl:ObjectProperty) 
 [![](../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[hasEventStatus](../Submissions/CommunicationEvent/hasEventStatus.md "Submissions:CommunicationEvent/hasEventStatus") page_
[![Class](../../../../../../../../../../../../../../../../../../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif.md "Class") __CommunicationEventStatus__ (owl:Class) The status of an event, e.g. suspended, started, ongoing, planned, proposed. 
 [![](../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[CommunicationEventStatus](../Submissions/CommunicationEvent/CommunicationEventStatus.md "Submissions:CommunicationEvent/CommunicationEventStatus") page_
[![ObjectProperty](../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __statusOfEvent__ (owl:ObjectProperty) 
 [![](../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[statusOfEvent](../Submissions/CommunicationEvent/statusOfEvent.md "Submissions:CommunicationEvent/statusOfEvent") page_
[![ObjectProperty](../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __isDurationOfEvent__ (owl:ObjectProperty) 
 [![](../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[isDurationOfEvent](../Submissions/CommunicationEvent/isDurationOfEvent.md "Submissions:CommunicationEvent/isDurationOfEvent") page_
[![ObjectProperty](../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif.md "ObjectProperty") __isDurationOfRelationship__ (owl:ObjectProperty) 
 [![](../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[isDurationOfRelationship](../Submissions/CommunicationEvent/isDurationOfRelationship.md "Submissions:CommunicationEvent/isDurationOfRelationship") page_
[![DatatypeProperty](../../../../images/thumb/a/a5/DatatypeProperty.gif/20px-DatatypeProperty.gif)](../Image/DatatypeProperty.gif.md "DatatypeProperty") __relationshipEndTime__ (owl:DatatypeProperty) 
 [![](../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[relationshipEndTime](../Submissions/CommunicationEvent/relationshipEndTime.md "Submissions:CommunicationEvent/relationshipEndTime") page_
[![DatatypeProperty](../../../../images/thumb/a/a5/DatatypeProperty.gif/20px-DatatypeProperty.gif)](../Image/DatatypeProperty.gif.md "DatatypeProperty") __eventEndTime__ (owl:DatatypeProperty) 
 [![](../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif.md "ArrowRight.gif") _[eventEndTime](../Submissions/CommunicationEvent/eventEndTime.md "Submissions:CommunicationEvent/eventEndTime") page_
#  Additional information


#  Scenarios



__Scenarios about CommunicationEvent__
No scenario is added to this Content OP.




#  Reviews



__Reviews about CommunicationEvent__
This revision (revision ID __10036__) takes in account the reviews: none


Other info at [evaluation tab](http://ontologydesignpatterns.org/wiki/index.php?title=Submissions:CommunicationEvent&action=evaluation "http://ontologydesignpatterns.org/wiki/index.php?title=Submissions:CommunicationEvent&action=evaluation")




  




#  Modeling issues



__Modeling issues about CommunicationEvent__
There is no Modeling issue related to this proposal.




  




#  References


[Add a reference](index.php@title=Odp%253AAdd_reference&subject=../Submissions/CommunicationEvent.md "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_reference&subject=Submissions%3ACommunicationEvent")





Retrieved from "[http://ontologydesignpatterns.org/wiki/Submissions:CommunicationEvent](../Submissions/CommunicationEvent.md)"
 [Categories](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [ProposedContentOP](../Category/ProposedContentOP.md "Category:ProposedContentOP") | [Review assigned](../Category/Review_assigned.md "Category:Review assigned")