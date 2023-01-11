[![](../images/thumb/6/6f/Definition.gif/70px-Definition.gif)](../Image/Definition.gif.md "Definition.gif")
__Logical Ontology Design Patterns (Logical OPs)__

A Logical OP is a formal expression, whose only parts are expressions from a logical vocabulary, e.g. OWL DL, that solves a problem of expressivity.


  



  




##   Description


Logical OPs are only expressed in terms of a logical vocabulary, because their
signature (the set of predicate names, e.g. the set of classes and properties in
an OWL ontology) is empty (with minor exceptions, e.g. the default inclusion
of owl:Thing in OWL). On one hand, Logical OPs are independent from a
specific domain of interest (i.e. they are content-independent), on the other
hand, they depend on the expressivity of the logical formalism that is used
for representation. In other words, Logical OPs help to solve design problems
where the primitives of the representation language do not directly support
certain logical constructs. For example, if the representation language is OWL,
and a designer needs to represent a relation between more than two elements,
a Logical OP is needed in order to express an n-ary relation semantics by
only using class and binary relation primitives. They can be of two types: logical macros, and transformation patterns.


Logical macros provide a "shortcut" to model a recurrent intuitive logical expression. Example: the macro ∇R.C colloquially means “every R must be a C” and 
formally ∃R.⊤ ⨅ ∀R.C which in OWL would be expressed as the combination of an owl:allValuesFrom restriction with an owl:someValuesFrom restriction.


Transformation patterns translate a logical expression from one logical language into another. 
The semantics of the ﬁrst is approximated, in order to ﬁnd a trade-off between requirements and expressivity. An example is N-ary relations that cannot be directly expressed in OWL. An approximation of an N-ary relation in OWL is to create a new class representing the relation and indicate the arguments through properties.





## Subcategories


This category has the following 2 subcategories, out of 2 total.


### C


* [CertifiedLogicalOP](../Category/CertifiedLogicalOP.md "Category:CertifiedLogicalOP")

### P


* [ProposedLogicalOP](../Category/ProposedLogicalOP.md "Category:ProposedLogicalOP")



## Pages in category "LogicalOP"


The following 18 pages are in this category, out of 18 total.




Retrieved from "[http://ontologydesignpatterns.org/wiki/Category:LogicalOP](../Category/LogicalOP.md)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [StructuralOP](../Category/StructuralOP.md "Category:StructuralOP")