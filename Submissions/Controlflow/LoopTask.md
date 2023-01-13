___LoopTask__ has [Category:OntologyElement](../../Category/OntologyElement.md "Category:OntologyElement") and is an [element of](../../Property/ElementOf.md "Property:ElementOf") [Controlflow](../../Submissions/Controlflow.md "Submissions:Controlflow")_


  




[![Class](../../images/thumb/2/27/Class.gif/45px-Class.gif)](../../Image/Class.gif.md "Class")
__Name__: LoopTask 


__Type:__ owl:Class 


__Description__: A loop task is a control task that has as successor an action -or complex- task that sequences at least two distinct activities sharing a minimal common set of properties -they have a MinimalCommonType. Notice that MinimalCommonType cannot be formalised as a first-order predicate, and then neither in OWL-DL. It can be considered a trivial guideline: when sequencing looped actions, choose a definite action class from the ground ontology.


Some relations typically hold for loop tasks. Exit condition can be used to state what deliberation task causes to exit the cycle; iteration interval can be used to state how much time should be taken by each iteration of the looped activity; iteration cardinality can be used to state how many times the action should be repeated. 





Retrieved from "[http://ontologydesignpatterns.org/wiki/Submissions:Controlflow/LoopTask](../../Submissions/Controlflow/LoopTask.md)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [OntologyElement](../../Category/OntologyElement.md "Category:OntologyElement")