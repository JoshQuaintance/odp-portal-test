#  Tasks/InfoTip broken for URI field


__Title:__ InfoTip broken for some fields


__Description:__ The property names OWLImplementation in the InfoTip for the URI field of the Edit\_Ontology form does not display. It is exactly the same syntax as the others that work fine. Indeed, you can replace the text "OWLImplementation" with "Description" and it displays fine. Maybe something about the name: OWLImplementation? It also does not work for some new properties I created: OntologyAuthor, OntologyOrganization and others.
See: [http://ontologydesignpatterns.org/wiki/Form:Edit\_Ontology](../../Form/Edit_Ontology.md "http://ontologydesignpatterns.org/wiki/Form:Edit_Ontology")


  





* __Type__: Bugfix
* __Posted by__: [MichaelUschold](../../User/MichaelUschold.md "User:MichaelUschold")
* __Status__: fixed


* __Priority__: Medium




__Sub-tasks__:
This task has no sub-tasks




[Development](../../Odp/Development.md "Odp:Development") | [Create new task](http://ontologydesignpatterns.org/wiki/Special:AddData/Task_Form?Task Template[SubmittedBy]=93.34.113.67).| [Add sub-task](http://ontologydesignpatterns.org/wiki/Special:AddData/Task_Form?parenttask=Tasks/InfoTip_broken_for_URI_field&Task Template[ParentTask]=Tasks/InfoTip_broken_for_URI_field&Task Template[SubmittedBy]=93.34.113.67) | [Add a comment at the bottom of this page](../index.php@title=Odp%253AAdd_comment&target=Odp%253ATasks%252F../../Odp/Tasks/InfoTip_broken_for_URI_field.md#New_comment "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_comment&target=Odp:Tasks/InfoTip_broken_for_URI_field#New_comment")
#####  12-02-2010 [EnricoDaga](../../User/EnricoDaga.md "User:EnricoDaga") says:


The name of the property must be added at the beginning of the page, for example in this way:




```
<includeonly>[[Property:TextReference|TextReference]].</includeonly>
 This property indicates a non-web resource that can be used as reference source for the Content OP e.g., the ISBN of a book. The value of this property is of type [[has type::Type:Text]].

```

  






Retrieved from "[http://ontologydesignpatterns.org/wiki/Odp:Tasks/InfoTip\_broken\_for\_URI\_field](../../Odp/Tasks/InfoTip_broken_for_URI_field.md)"
 [Categories](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [RootTask](../../Category/RootTask.md "Category:RootTask") | [DevelopmentTask](../../Category/DevelopmentTask.md "Category:DevelopmentTask")