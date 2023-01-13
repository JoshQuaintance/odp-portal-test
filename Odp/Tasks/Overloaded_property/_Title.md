#  Tasks/Overloaded property: Title


__Title:__ InfoTip text inaccurate for Title field of modeling issues


__Description:__ The infotip for the title field on the [Modeling Issue Form](../../../Form/Modeling_Issue_Form "Form:Modeling Issue Form") is wrong. It says the field will be used for the title of the wiki page. That was true on the create page, but is not true here. The "title" field does not change the page title. It just give a way to have a name that is different from the title. The easiest solution is probably to just re-use the [name property](../../../Property/Name "Property:Name") that is also used in the exemplary ontology form. A alternative solution is to have a new property, e.g. IssueTitle with new help text. 


Data migration will have to happen carefully. This is similar to two other tasks for creating Issue. This is similar to the task: [RelatedCP property overloaded](../../../Odp/Tasks/RelatedCP_property_overloaded "Odp:Tasks/RelatedCP property overloaded")


  





* __Type__: Bugfix
* __Posted by__: [MichaelUschold](../../../User/MichaelUschold "User:MichaelUschold")
* __Status__: To be done


* __Priority__: Medium




__Sub-tasks__:
This task has no sub-tasks




[Development](../../../Odp/Development "Odp:Development") | [Create new task](http://ontologydesignpatterns.org/wiki/Special:AddData/Task_Form?Task Template[SubmittedBy]=93.34.113.67).| [Add sub-task](http://ontologydesignpatterns.org/wiki/Special:AddData/Task_Form?parenttask=Tasks/Overloaded_property:_Title&Task Template[ParentTask]=Tasks/Overloaded_property:_Title&Task Template[SubmittedBy]=93.34.113.67) | [Add a comment at the bottom of this page](../index.php@title=Odp%253AAdd_comment&target=Odp%253ATasks%252F../../../Odp/Tasks/Overloaded_property/_Title#New_comment "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_comment&target=Odp:Tasks/Overloaded_property:_Title#New_comment")
#####  1-03-2010 [EnricoDaga](../../../User/EnricoDaga "User:EnricoDaga") says:


If the Title property is aligned with the page title at creation, we can remove the possibility to change it in editing.


The Title property can have as value the name of the page, so if the user moves the page the property is updated automatically.


In this way the property and the page title will remain aligned.


But if we see an added value to have a name property independent from the page title, we can add a 'Name' property, or refactor the 'Title' property in modelling issues.


So options are:



1. Let the Title property be aligned with the page name (and forbid manual editing).
2. Refactor the 'Title' property with a 'Name' property.


  




#####  1-03-2010 [EnricoDaga](../../../User/EnricoDaga "User:EnricoDaga") says:


I have noted that the Modeling issue page uses the _TitleDescription Template_ template.


This template is used also in other page models (Feedbacks, for example)


This means that a refactoring of the property 'Title' cannot be done.


Options are:



1. Let the Title property be aligned with the page name (and forbid manual editing)
2. The page must not use the _TitleDescription Template_. This template can be substituted with another one, _NameDescription_ that uses 'Name' insteadof 'Title'.




Retrieved from "[http://ontologydesignpatterns.org/wiki/Odp:Tasks/Overloaded\_property:\_Title](../../../Odp/Tasks/Overloaded_property/_Title)"
 [Categories](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [RootTask](../../../Category/RootTask "Category:RootTask") | [DevelopmentTask](../../../Category/DevelopmentTask "Category:DevelopmentTask")