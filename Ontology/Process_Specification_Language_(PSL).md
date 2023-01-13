Return to [Catalogue of Exemplary Ontologies](../Ontology/Main.md "Ontology:Main")



#  Ontology Overview


#  Long Description


For many years, the [Manufacturing Systems Integration Division](http://www.nist.gov/msid/ "http://www.nist.gov/msid/") (MSID) has been involved in the definition of a neutral representation of product data, most recently realized through the STEP standard. With that effort well underway, another candidate area for a division focus is the representation of manufacturing process. Like product data, process data is also used throughout the life cycle of a product, from early indications of manufacturing process flagged during design, through process planning, validation, production scheduling and control. In addition, the notion of process also underlies the entire manufacturing cycle, coordinating the workflow within engineering and shop floor manufacturing. 


The Process Specification Language (PSL) defines a neutral representation for manufacturing processes that supports automated reasoning. Process data is used throughout the life cycle of a product, from early indications of manufacturing process flagged during design, through process planning, validation, production scheduling and control. In addition, the notion of process also underlies the entire manufacturing cycle, coordinating the workflow within engineering and shop floor manufacturing. 


If you would like to learn more about PSL, including rationale and the need for its implementation, please [click here](http://www.mel.nist.gov/psl/rationale.html "http://www.mel.nist.gov/psl/rationale.html"). 



###   PSL Ontology -- Current Theories and Extensions (version 2.8)


The axioms of PSL are organized into PSL-Core and a set of extensions. PSL-Core is the set of axioms written in CLIF (the [Common Logic](http://www.nist.gov/cgi-bin/exit_nist.cgi?url=http://philebus.tamu.edu/cl/ "http://www.nist.gov/cgi-bin/exit_nist.cgi?url=http://philebus.tamu.edu/cl/") Interchange Format) and using only the nonlogical lexicon of PSL-Core. The extensions form a lattice of extensions to PSL-Core. 


The purpose of PSL-Core is to axiomatise a set of intuitive semantic primitives that is adequate for describing the fundamental concepts of manufacturing processes. Consequently, this characterization of basic processes makes few assumptions about their nature beyond what is needed for describing those processes, and the Core is therefore rather weak in terms of logical expressiveness. In particular, PSL-Core is not strong enough to provide definitions of the many auxiliary notions that become necessary to describe all intuitions about manufacturing processes. 


To supplement the concepts of PSL-Core, the ontology includes a set of extensions that introduce new terminology. An PSL extension provides the logical expressiveness to express information involving concepts that are not explicitly specified in PSL-Core. For each symbol in the nonlogical lexicon of an extension of PSL, there exist one or more axioms, written in CLIF, that constrain its interpretation. A distinction is drawn between definitional and nondefinitional extensions of PSL-Core. A definitional extension is an extension whose nonlogical lexicon can be completely defined in terms of PSL-Core. Definitional extensions add no new expressive power to PSL-Core. Nondefinitional extensions (also called core theories) are extensions of PSL-Core that involve at least one new primitive not contained in PSL-Core. All extensions within PSL must be consistent extensions of PSL-Core, and may be consistent extensions of other PSL extensions. However, not all extensions within PSL need be mutually consistent.


The organization of the extensions below reflects the Parts within standard [ISO 18629](http://www.nist.gov/cgi-bin/exit_nist.cgi?url=http://www.iso.org/iso/en/CatalogueDetailPage.CatalogueDetail?CSNUMBER=35185&ICS1=25&ICS2=40&ICS3=40 "http://www.nist.gov/cgi-bin/exit_nist.cgi?url=http://www.iso.org/iso/en/CatalogueDetailPage.CatalogueDetail?CSNUMBER=35185&ICS1=25&ICS2=40&ICS3=40"). All files are updates to the standard, except for those marked by â€œxâ€, which are in progress. Other status indicators are: â€œcâ€ (consistency proof completed) and â€œcaâ€ (consistency verified by the automated theorem prover [Vampire](http://www.nist.gov/cgi-bin/exit_nist.cgi?url=http://en.wikipedia.org/wiki/Vampire_theorem_prover "http://www.nist.gov/cgi-bin/exit_nist.cgi?url=http://en.wikipedia.org/wiki/Vampire_theorem_prover")). The syntax of all files has been checked by automated theorem provers, see [download page](http://www.mel.nist.gov/psl/download.html "http://www.mel.nist.gov/psl/download.html"). 


  

The purpose of PSL-Core is to axiomatize a set of intuitive semantic primitives that is adequate for describing the fundamental concepts of manufacturing processes. Consequently, this characterization of basic processes makes few assumptions about their nature beyond what is needed for describing those processes, and the Core is therefore rather weak in terms of logical expressiveness.


The basic ontological commitments of PSL-Core are based on the following intuitions:


__Intuition 1:__


_There are four kinds of entities required for reasoning about processes -- activities, activity occurrences, timepoints, and objects._ 


__Intuition 2:__


_Activities may have multiple occurrences, or there may exist activities that do not occur at all._ 


__Intuition 3:__


_Timepoints are linearly ordered, forwards into the future, and backwards into the past._ 


__Intuition 4:__


_Activity occurrences and objects are associated with unique timepoints that mark the begin and end of the occurrence or object._ 



###   Key Publications


Bock, C. and Gruninger, M. (2004) [PSL: A semantic domain for flow models](http://stl.mie.utoronto.ca/publications/semantic_domain.pdf "http://stl.mie.utoronto.ca/publications/semantic_domain.pdf"), __Software and Systems Modeling__. 


  

Gruninger, M. and Menzel, C. (2003)[Process Specification Language: Principles and Applications](http://stl.mie.utoronto.ca/publications/psl-aimag.pdf "http://stl.mie.utoronto.ca/publications/psl-aimag.pdf"), __AI Magazine__, 24:63-74. 


  

Cheng, J., Gruninger, M., Sriram, R., and Law, K. (2003)[Process Specification Language for project scheduling information exchange](http://stl.mie.utoronto.ca/publications/pslschedules.pdf "http://stl.mie.utoronto.ca/publications/pslschedules.pdf"), __International Journal of IT in Architecture, Engineering and Construction__, 1:307-328.



#  Additional Information


  



  




#  References


[Add a reference](index.php@title=Odp%253AAdd_reference&subject=Ontology%253AProcess+Specification+Language+(PSL).html "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_reference&subject=Ontology%3AProcess+Specification+Language+%28PSL%29")



* PSL Downloads [Downloads](http://www.mel.nist.gov/psl/download.html "http://www.mel.nist.gov/psl/download.html") | [reference page](../Community/References/PSL_Downloads.md "Community:References/PSL Downloads")
* Bock, C. and Gruninger, M. (2004) PSL: A semantic domain for flow models, Software and Systems Modeling. [Paper](http://stl.mie.utoronto.ca/publications/semantic_domain.pdf "http://stl.mie.utoronto.ca/publications/semantic_domain.pdf") | [reference page](../Community/References/PSL_for_flow_models.md "Community:References/PSL for flow models")
* Gruninger, M. and Menzel, C. (2003)The Process Specification Language: Theory and Applications, AI Magazine, 24:63-74. [Paper](http://stl.mie.utoronto.ca/publications/psl-aimag.pdf "http://stl.mie.utoronto.ca/publications/psl-aimag.pdf") | [reference page](../Community/References/PSL_AIMAG.md "Community:References/PSL AIMAG")
* Cheng, J., Gruninger, M., Sriram, R., and Law, K. (2003)Process Specification Language for project scheduling information exchange, International Journal of IT in Architecture, Engineering and Construction, 1:307-328. [Paper](http://stl.mie.utoronto.ca/publications/pslschedules.pdf "http://stl.mie.utoronto.ca/publications/pslschedules.pdf") | [reference page](../Community/References/PSL-Schedule.md "Community:References/PSL-Schedule")
* PSL Home Page [Project Home Page](http://www.mel.nist.gov/psl/ "http://www.mel.nist.gov/psl/") | [reference page](../Community/References/PSL_Home_Page.md "Community:References/PSL Home Page")




Retrieved from "[http://ontologydesignpatterns.org/wiki/Ontology:Process\_Specification\_Language\_%28PSL%29](../Ontology/Process_Specification_Language_(PSL).md).md).html)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [Ontology](../Category/Ontology.md "Category:Ontology")