[![](../images/thumb/2/29/Reviewer.png/48px-Reviewer.png)](../Image/Reviewer.png "Reviewer.png")
__[BenedictoRodriguezCastro](../User/BenedictoRodriguezCastro "User:BenedictoRodriguezCastro") about [TransportPattern](../Submissions/TransportPattern "Submissions:TransportPattern") (Revision ID: [11661](../Submissions/TransportPattern@oldid=11661 "http://ontologydesignpatterns.org/wiki/Submissions:TransportPattern?oldid=11661"))__
Overall suggestion (score): 0 - needs major revision




 __Review Summary:__ Note to Program Committee:
This "Review Summary" is the same as uploaded to EasyChair based on the 4.5 pages paper submitted by the authors. The rating of -1 (weak accept) on EasyChair or 0 (needs minor revision) here is based on the content of the paper. The content submitted on this Web portal for this pattern is very poor and leans toward a rating of -1 (reject).


---


Note to authors: 


PLEASE, POPULATE THE CONTENTS OF THE PAPER ON THE CORRESPONDING FIELDS ON THE SUBMISSION PAGE OF THIS WEB PORTAL.


---


This pattern submission introduces an Ontology Design Pattern (ODP) for the concept of "Transport" in the domain of Geosciences. The meaning of the concept of "Transport" intended to be modeled is defined. The main elements of the pattern are introduced together with their role and function. The pattern is characterized in general terms so that it could be applied to other domains as well. The authors provide an example of how some of the core elements of the pattern can be extended to represent additional aspects associated with the notion of a "transport event".


The strengths and weaknesses of the submission are summarized below:


- The Transport ODP is highly relevant to the workshop because the topics discussed fall well within the scope of the WOP event.


- The readability of the submission is clear. The originality and contribution of the pattern can be seen as novel because, although anchored as an extension to the Semantic Web for Earth and Environmental Terminology (SWEET) ontology, the proposed representation of the concept of "Transport" as defined in the submission, is new.


- The discussion of related work can be significantly improved because, although the submission mentions other ontologies that the pattern extends (i.e. SWEET) or that it can be linked to (i.e. SOS, or GML), it does not state explicitly whether there have been (or not) previous efforts at representing in a Web ontology, the same notion of "Transport" put forward by the authors. 


- The potential practical utility of the proposed approach is very promising because the pattern is defined in general terms and its representation of a "transport event" could be applied to many domains. However, the documentation of the pattern in the submission hampers its utility because there is not a simple full example of a "transport event" illustrating the instantiation of all elements of the pattern. Some "transport event" examples are mentioned (i.e. river flow, air travel) but the instantiation of the pattern is left to the intuition of the reader. Other examples stated can be complex for those not familiar with their particular domain (osmosis, diffusion, etc.).


- The generic schema of the pattern, the naming convention of the core elements and its graphical representations are misleading or unclear because: 
(a) the names given in the narrative do not align the names given to the corresponding object in the figure (i .e. transportEvent, vs. TransportEvent or referenceFrame vs. ReferenceFrame - which one is it?); 
(b) the same object in the figure is used to represent classes and properties (both Transport-, and ReferenceFrame are round boxes); 
(c) what does the arrow "propertyOf" in Figure 1 represents? It is not addressed; 
(d) what do the different colors chosen in Figure 2 represent? and 
(e) the choice of the "partOf" relation between core classes in the pattern is never discussed.


- The implementation of the pattern provided in [1] seems to contain a bug, likely due to the naming issues identified above. The domain and range in the definition of the property :referenceFrame in [1] is set to the URI :transportEvent (low-case 't'), which is not explicitly defined as a class in the .owl file. However, the URI :TransportEvent (upper-case 'T') is.


[1] [https://wiki.auckland.ac.nz/download/attachments/52016791/TransportPattern.owl](https://wiki.auckland.ac.nz/download/attachments/52016791/TransportPattern.owl "https://wiki.auckland.ac.nz/download/attachments/52016791/TransportPattern.owl")


- In terms of evaluation, the authors acknowledged how it could be approached but as stated earlier, there are no clear or real concrete examples of full instantiations of the pattern. Figure 2 suggests how the pattern can be populated or extended but the concepts used (osmosis, diffusion, percolation, etc.) may not be the ideal introductory example as they represent very specific domains and certain degree of experience in them may be required.



Overall, a very interesting pattern for a modeling scenario (a transport event) very prevalent in the real world. Even though there are several aspects of the pattern that should be improved in terms of documentation and exemplification as outlined above, the essential conceptualization of the pattern is valid and it could prove an interesting point of discussion at the WOP event. Thus, the recommended rating is 0 (needs major revision) (which I am equating to a -1 -weak reject- on EasyChair).
__Reviewer Confidence:__ - The confidence level regarding the OWL idioms involved in the pattern is high. 
- The confidence level of the application domain as it is discussed in the paper submission (transport event, active/passive transport, etc.) is fair.
__Problems:__ See section "Review Summary".
__Community Relevance:__ See section "Review Summary".
__Relation to Best Practices:__ See section "Review Summary".
__Reusability:__ See section "Review Summary".
__Relations to Other Patterns:__ See section "Review Summary".
__Overall Understandability:__ See section "Review Summary".
__Clear Problem Description:__ See section "Review Summary".
__Clear Relevance and Consequences:__ See section "Review Summary".
__Clear Figures and Illustrations:__ See section "Review Summary".
__Missing Information:__ See section "Review Summary".

_Posted:_ 2013/8/10 _Last modified:_ 2013/8/10



[All reviews](../Reviews/Main "Reviews:Main") | [Add a comment at the bottom of this page](index.php@title=Odp%253AAdd_comment&target=../Reviews/BenedictoRodriguezCastro_about_TransportPattern#New_comment "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_comment&target=Reviews:BenedictoRodriguezCastro_about_TransportPattern#New_comment")


Retrieved from "[http://ontologydesignpatterns.org/wiki/Reviews:BenedictoRodriguezCastro\_about\_TransportPattern](../Reviews/BenedictoRodriguezCastro_about_TransportPattern)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [QCReview](../Category/QCReview "Category:QCReview")