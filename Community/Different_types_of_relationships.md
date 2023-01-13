#  Different types of relationships


__Title:__ Different types of relationships for ontology representation


__Description:__ In real applications, we need a flexible ontology editor that helps the user represent taxonomies based on different types of relationships between concepts and with specific features, constraints and rules for each type of relationship. E.g., specialization (is-a) taxonomies, composition (part-whole) taxonomies, lists, etc. The reason is that some features for the specialization taxonomies (represented by the existing editors, e.g., the property inheritance) are not always appropriate for taxonomies based on other types of relationships.
Also, the editor should be flexible enough to represent taxonomies based on new types of relationships and specific features, proposed by the user.
Our solution for a project in progress was to build an editor that allows the user choose the type of taxonomy and that automatically applies the property inheritance only for the specialization taxonomies. For the composition taxonomies, the concept properties are inherited on demand. And for the list-like taxonomies the inheritance is applicable only for properties defined at the ontology level (inherited by all concepts). The editor is not yet flexible enough to help the user add taxonomies based on new relationship types and with features he needs for an application. 


__Diagram__
_(this article has no graphical representation)_



#  About


  




#  Additional information


#  References


[Add a reference](index.php@title=Odp%253AAdd_reference&subject=Community%253ADifferent+types+of+relationships.html "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_reference&subject=Community%3ADifferent+types+of+relationships")


  




 [List of Modeling Issues](../Community/Main "Community:Main") | [Post a new modeling issue](../Community/PostModelingIssue "Community:PostModelingIssue") | [Add a comment in the discussion page](index.php@title=Odp%253AAdd_comment&target=Community_talk%253ADifferent_types_of_relationships.html#New_comment "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_comment&target=Community_talk:Different_types_of_relationships#New_comment")


Retrieved from "[http://ontologydesignpatterns.org/wiki/Community:Different\_types\_of\_relationships](../Community/Different_types_of_relationships)"
 [Categories](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [ModelingIssue](../Category/ModelingIssue "Category:ModelingIssue") | [Submitted to event](../Category/Submitted_to_event "Category:Submitted to event")