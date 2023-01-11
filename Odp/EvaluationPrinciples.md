[Certified Content ODPs (CPs)](../Category/CertifiedContentOP.md "Category:CertifiedContentOP") must comply to a set of criteria and requirements described below.


Members of the  [Quality Committee](../QualityCommittee.md "QualityCommittee") use them in order to review and certify  [Proposed Content ODPs](../Category/ProposedContentOP.md "Category:ProposedContentOP").


Such criteria can also be useful as guidelines for those who want to [propose a Content ODP](../Submissions/ProposeCP.md "Submissions:ProposeCP").



##   Criteria


* __Computational components__. CPs are language-independent, and should be encoded in a higher-order representation language. Nevertheless, their (sample) representation in OWL is needed in order to (re)use them as _building blocks_ over the Semantic Web.


* __Requirements covering components__. A CP is deﬁned in terms of the requirements it satisﬁes, which are expressed in terms of competency questions. This aspects is also important for stating the relevance of the CP with reference to a certain  [domain](../Community/Domain.md "Community:Domain").


* __Small, autonomous components__. Regardless of the particular way a CP has been created it is a small, autonomous ontology. Smallness and autonomy of CPs facilitate ontology designers: composing CPs enable them to govern the complexity of the whole ontology, because of the explicit rationales and the amount of know-how provided by the users of a same CP library. Smallness also allows diagrammatical visualizations that are aesthetically acceptable and easily memorizable.


* __Hierarchical components__. A CP can be an element in a partial order, where the ordering relation requires that at least one of the classes or properties in the pattern is either specialized or generalized. A hierarchy of CPs can be built by specializing or generalizing some of the elements (either classes or relations).


* __Cognitively relevant components__. CP visualization must be intuitive and compact, and should catch relevant, _core_ notions of a  [domain](../Community/Domain.md "Community:Domain"). An interesting result from cognitive learning is that the development of expert skills typically _selects_ patterns of concepts that are richly interconnected, and in normal cases, these patterns are applied without an explicit reference to the underlying detailed knowledge acquired during the training period. This result matches the need to quickly reason or to automatize cer tain tasks, and the experimental data on short-term memory capacity. For this reason, independently of the generality at which a CP is singled out, it must contain the central notions that _make rational thinking move_ for an expert in a given  [domain](../Community/Domain.md "Community:Domain") for a given task.


* __Reasoning relevant components__. A CP has to allow some form of inference.


* __Linguistically relevant components__. Many CPs nicely match linguistic patterns called frames. A frame can be described as a lexically founded ontology design pattern; frames typically encode argument structures for verbs, e.g. the frame Desiring associates elements (or semantic roles) such as Experiencer, Event, FocalParticipant, LocationOfEvent, etc. The richest repository of frames is [FrameNet](http://framenet.icsi.berkeley.edu/ "http://framenet.icsi.berkeley.edu/"). Frames can be used for validating CPs with respect to lexical coverage, for lexicalizing them, and can be reengineered in order to populate the CP catalogue.


* __Best practice components__. A CP should be used to describe a good practice of modelling. Good practices are intended here as local, thus derived from experts. The quality of CPs is currently based on the personal experience and taste of the proposers, or on the provenance of the knowledge resource where the CP comes from. However, evidence from reusability across different projects, large-scale applications, and open rating systems will provide a good base for CP evaluation.


##   Requirements


* Each CP must be associated with: an OWL implementation, at least one OWL instantiation example, a UML diagram, the description of all its ontology elements, the domain, at least one competency question and one scenario, a source model from which it has been extracted/reengineered from.
* The CP OWL implementation has to be annotated by means of the [ODP CP annotation schema](http://www.ontologydesignpatterns.org/schemas/cpannotationschema.owl "http://www.ontologydesignpatterns.org/schemas/cpannotationschema.owl")




Retrieved from "[http://ontologydesignpatterns.org/wiki/Odp:ContentODPEvaluationPrinciples](../Odp/ContentODPEvaluationPrinciples.md)"