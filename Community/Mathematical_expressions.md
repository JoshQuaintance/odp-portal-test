#  Mathematical expressions


__Title:__ Representing in OWL mathematical expressions.


__Description:__ I wish to be able to express:
- "gross income" calculatedBy ("yield" multipliedBy "price")
- "net income" calculatedBy ("gross income" minus " cost product") 


__Diagram__
_(this article has no graphical representation)_



#  About


  




#  Additional information


Proposed by Aldo:


GrossIncome equivalentClass




```
 (NumericProduct and
 (hasFirstOperand some Yield) and
 (hasSecondOperand some Price)
 (hasResult exactly 1))

```

GrossIncome subClassOf




```
 hasFirstOperand all Yield

```

GrossIncome subClassOf




```
 hasSecondOperand all Price

```

GrossIncome subClassOf




```
 hasResult all xsd:float

```

Yield subClassOf




```
 hasValue some xsd:float

```

Price subClassOf




```
 hasValue some xsd:float

```

Proposed by Margherita (simpler version):


<rdf:RDF




```
   xmlns="[http://localhost/default#](http://localhost/default# "http://localhost/default#")"
   xmlns:rdf="[http://www.w3.org/1999/02/22-rdf-syntax-ns#](http://www.w3.org/1999/02/22-rdf-syntax-ns# "http://www.w3.org/1999/02/22-rdf-syntax-ns#")"
   xmlns:xsd="[http://www.w3.org/2001/XMLSchema#](http://www.w3.org/2001/XMLSchema# "http://www.w3.org/2001/XMLSchema#")"
   xmlns:rdfs="[http://www.w3.org/2000/01/rdf-schema#](http://www.w3.org/2000/01/rdf-schema# "http://www.w3.org/2000/01/rdf-schema#")"
   xmlns:owl="[http://www.w3.org/2002/07/owl#](http://www.w3.org/2002/07/owl# "http://www.w3.org/2002/07/owl#")"
   xmlns:daml="[http://www.daml.org/2001/03/daml+oil#](http://www.daml.org/2001/03/daml+oil# "http://www.daml.org/2001/03/daml+oil#")">
 <owl:Class rdf:about="[http://localhost/default#Numeric%20Product](http://localhost/default#Numeric%20Product "http://localhost/default#Numeric%20Product")">
   <hasSecondOperand>
     <owl:Class rdf:about="[http://localhost/default#Price](http://localhost/default#Price "http://localhost/default#Price")"/>
   </hasSecondOperand>
   <hasFirstOperand>
     <owl:Class rdf:about="[http://localhost/default#Yield](http://localhost/default#Yield "http://localhost/default#Yield")"/>
   </hasFirstOperand>
 </owl:Class>
 <owl:Class rdf:about="[http://localhost/default#Multiplication](http://localhost/default#Multiplication "http://localhost/default#Multiplication")">
   <rdfs:subClassOf>
     <owl:Class rdf:about="[http://localhost/default#Arithmetic%20operand](http://localhost/default#Arithmetic%20operand "http://localhost/default#Arithmetic%20operand")"/>
   </rdfs:subClassOf>
 </owl:Class>
 <owl:Class rdf:about="[http://localhost/default#Gross%20Income](http://localhost/default#Gross%20Income "http://localhost/default#Gross%20Income")"/>
 <owl:ObjectProperty rdf:about="[http://localhost/default#hasOperand](http://localhost/default#hasOperand "http://localhost/default#hasOperand")">
   <rdfs:range rdf:resource="[http://localhost/default#Multiplication](http://localhost/default#Multiplication "http://localhost/default#Multiplication")"/>
   <rdfs:domain rdf:resource="[http://localhost/default#Numeric%20Product](http://localhost/default#Numeric%20Product "http://localhost/default#Numeric%20Product")"/>
   <rdf:type rdf:resource="[http://www.w3.org/1999/02/22-rdf-syntax-ns#Property](http://www.w3.org/1999/02/22-rdf-syntax-ns#Property "http://www.w3.org/1999/02/22-rdf-syntax-ns#Property")"/>
 </owl:ObjectProperty>
 <owl:ObjectProperty rdf:about="[http://localhost/default#calculatedBy](http://localhost/default#calculatedBy "http://localhost/default#calculatedBy")">
   <rdfs:range rdf:resource="[http://localhost/default#Numeric%20Product](http://localhost/default#Numeric%20Product "http://localhost/default#Numeric%20Product")"/>
   <rdfs:domain rdf:resource="[http://localhost/default#Gross%20Income](http://localhost/default#Gross%20Income "http://localhost/default#Gross%20Income")"/>
   <rdf:type rdf:resource="[http://www.w3.org/1999/02/22-rdf-syntax-ns#Property](http://www.w3.org/1999/02/22-rdf-syntax-ns#Property "http://www.w3.org/1999/02/22-rdf-syntax-ns#Property")"/>
 </owl:ObjectProperty>

```

</rdf:RDF>



#  References


[Add a reference](index.php@title=Odp%253AAdd_reference&subject=Community%253AMathematical+expressions.html "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_reference&subject=Community%3AMathematical+expressions")


  




 [List of Modeling Issues](../Community/Main "Community:Main") | [Post a new modeling issue](../Community/PostModelingIssue "Community:PostModelingIssue") | [Add a comment in the discussion page](index.php@title=Odp%253AAdd_comment&target=Community_talk%253AMathematical_expressions.html#New_comment "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_comment&target=Community_talk:Mathematical_expressions#New_comment")


Retrieved from "[http://ontologydesignpatterns.org/wiki/Community:Mathematical\_expressions](../Community/Mathematical_expressions)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [ModelingIssue](../Category/ModelingIssue "Category:ModelingIssue")