[![](../images/thumb/2/29/Reviewer.png/48px-Reviewer.png)](../Image/Reviewer.png.md "Reviewer.png")
__[WimPeters](../User/WimPeters.md "User:WimPeters") about [ConceptTerms](../Submissions/ConceptTerms.md "Submissions:ConceptTerms") (Revision ID: [5626](../Submissions/ConceptTerms@oldid=5626.md "http://ontologydesignpatterns.org/wiki/Submissions:ConceptTerms?oldid=5626"))__
Overall suggestion (score): 1 - needs minor revision




 __Review Summary:__ Overall, this pattern constitutes a good candidate, because it is based on an existing standard. This indicates the need for the incorporation of more standard representations for this particular modeling issue in ODP. Only then a proper discussion of this pattern is possible. Until then, the fact that it bases itself on a standard warrants acceptance.
__Reviewer Confidence:__ My confidence is high for modeling the relation between linguistic/terminological knowledge and ontology classes.
__Problems:__ The pattern has been used in various scenarios, and is from that perspective interesting to discuss.
The model, which has been re-engineered directly from a terminological standard model, is too simple to express many linguistic notions that contribute to the quality of information extraction.
It is very important to acknowledge that the pattern fits into a range of proposed standard formats for the expression of concept labels in terms of preference and constitution, such as SKOS, TBX, TMF, LMF, LIR and LingInfo.



It is only after the inclusionof these patterns that it is possible to have a proper discussion of the merits of this pattern on the basis of a comprehensive comparison.
__Community Relevance:__ high for users adhering to the BS8723-2 standard. Insufficient for users who need to model more comples linguistic knowledge.
__Relation to Best Practices:__ The pattern does represent a best practise, since it is based on a standard.
There are may alternative solutions, which need to be modeled as alternatives, and linked to this pattern in order to maximize coverage and usage.
__Reusability:__ very re-usable, because of its modular nature.
__Relations to Other Patterns:__ other standards and best practises need to be proposed as alternatives.
__Overall Understandability:__ 
__Clear Problem Description:__ the description of the problem is
__Clear Relevance and Consequences:__ these are clearly stated.
__Clear Figures and Illustrations:__ Not sll relatons are named in the diagram, more specifically the relations involving terms.
__Missing Information:__ A scenario should be added, in which ideally all classes come into play, in order to show why this particular constellation of simple/compound (non)prefered terms is necessary versus a more straightforward list of components model from LMF (see [http://gate.ac.uk/gate-extras/neon/ontologies/Lmf-component-module.owl](http://gate.ac.uk/gate-extras/neon/ontologies/Lmf-component-module.owl "http://gate.ac.uk/gate-extras/neon/ontologies/Lmf-component-module.owl") and [http://ontoware.org/frs/download.php/606/lmf.owl](http://ontoware.org/frs/download.php/606/lmf.owl "http://ontoware.org/frs/download.php/606/lmf.owl")
The authors should be more specific about the way in which the re-engineering of this particular BS8723-2 fragment is incomplete.



It omits the Equivalence relation between SimpleNonPreferredTerm and PreferredTerm. Also, the CompoundEquivalence relation between PreferredTerm and CompoundNonPreferredTerm is lacking. The model is available from [http://schemas.bs8723.org/Model.aspx](http://schemas.bs8723.org/Model.aspx "http://schemas.bs8723.org/Model.aspx").

_Posted:_ 2009/9/8 _Last modified:_ 2009/9/8



[All reviews](../Reviews/Main.md "Reviews:Main") | [Add a comment at the bottom of this page](index.php@title=Odp%253AAdd_comment&target=../Reviews/WimPeters_about_ConceptTerms.md#New_comment "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_comment&target=Reviews:WimPeters_about_ConceptTerms#New_comment")


Retrieved from "[http://ontologydesignpatterns.org/wiki/Reviews:WimPeters\_about\_ConceptTerms](../Reviews/WimPeters_about_ConceptTerms.md)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [QCReview](../Category/QCReview.md "Category:QCReview")