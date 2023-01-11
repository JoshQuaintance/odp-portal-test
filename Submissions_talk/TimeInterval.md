While I agree with the general points of and the need for a standardised way of describing how to model time and intervals of time, I am curious as to why the W3C standard time ontology is not used instead ([http://www.w3.org/2006/time](http://www.w3.org/2006/time "http://www.w3.org/2006/time"), described at [http://www.w3.org/TR/owl-time/](http://www.w3.org/TR/owl-time/ "http://www.w3.org/TR/owl-time/")). It seems to me that using this standard would further interoperability more than reinventing the wheel by defining our own TimeInterval class and related properties, only for use within the ontologydesignpatterns.org pattern repository. Is there any particular reason as to why you've chosen to go this route?


/Karl Hammar


Having discussed with Eva Blomqvist, I now understand the origins of a lot of the ontologydesignpatterns.org patterns come from various upper level ontologies (DOLCE and DUL were mentioned), and if this is the case, it is of course natural that the way that time is modeled is also from one of these sources and therefore perhaps incompatible with the previously mentioned W3C Time ontology.


However, being interested in interoperability, I will when my current project is through look into creating some patterns that replicate the functions and features of the patterns in this repository, but use the W3C time classes instead. I think that a little bit of such unification could prove to be quite useful to the community.


/Karl Hammar





Retrieved from "[http://ontologydesignpatterns.org/wiki/Submissions\_talk:TimeInterval](../Submissions_talk/TimeInterval.md)"