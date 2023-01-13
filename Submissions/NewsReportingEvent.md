[![](../images/thumb/b/b5/Certified.png/70px-Certified.png)](../Image/Certified.png "Certified.png") __This pattern has been certified.__
Related submission, with evaluation history, can be found __here__





#  Graphical representation


__Diagram__




[![Image:ReportingNewsEvent-scheme.png](../images/d/d9/ReportingNewsEvent-scheme.png)](../Image/ReportingNewsEvent-scheme.png "Image:ReportingNewsEvent-scheme.png")




#  General description


  




#  Elements


_The __NewsReportingEvent__ Content OP locally defines the following ontology elements:_



[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif "ObjectProperty") __hasPresentationContext__ (owl:ObjectProperty) This property can be used to link NewsReportingEvent to a NewsPresentationContext. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[hasPresentationContext](../Submissions/NewsReportingEvent/hasPresentationContext "Submissions:NewsReportingEvent/hasPresentationContext") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif "ObjectProperty") __owns__ (owl:ObjectProperty) This property can be used to link a certain NewsProvider with a Media that the NewsProvider ows, e.g. Fox News Channel is owned by Fox Entertainment Group, which also owns other Media (FXX Channel, etc.).
This is an universal property, it can be also used in different context (e.g. Ruslana owns a Persian cat). 



 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[owns](../Submissions/NewsReportingEvent/owns "Submissions:NewsReportingEvent/owns") page_
[![ObjectProperty](../images/thumb/c/c3/ObjectProperty.gif/20px-ObjectProperty.gif)](../Image/ObjectProperty.gif "ObjectProperty") __presentedAt__ (owl:ObjectProperty) This property can be used to link a NewsReportingEvent to a Media (TV station, radio station, newspaper, webpage) at which a certain ActualEventView was presented. 
This is an universal property and can be used in different contexts. 



 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[presentedAt](../Submissions/NewsReportingEvent/presentedAt "Submissions:NewsReportingEvent/presentedAt") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif "Class") __Media__ (owl:Class) An entity that allows a communication of news messages, for example a TV station, radio station, newspaper, website, etc. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[Media](../Submissions/NewsReportingEvent/Media "Submissions:NewsReportingEvent/Media") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif "Class") __NewsEventReporter__ (owl:Class) An Actor (usually a Person) that is an author of a certain ActualEventView.
NewsEventReporter is not linked to an ActualEventView directly, it is connected to NewsReportingEvent, which is designed to document the act of reporting. 



 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[NewsEventReporter](../Submissions/NewsReportingEvent/NewsEventReporter "Submissions:NewsReportingEvent/NewsEventReporter") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif "Class") __NewsPresentationContext__ (owl:Class) Class for denoting circumstances of an actual event presentation. For example if an event was presented at the end of website, then end of website is its NewsPresentationContext.
NewsPresentationContext is not directly attached to an ActualEventView, it is attached to NewsReportingEvent, which designates the act of an event reporting. 



 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[NewsPresentationContext](../Submissions/NewsReportingEvent/NewsPresentationContext "Submissions:NewsReportingEvent/NewsPresentationContext") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif "Class") __NewsProvider__ (owl:Class) An entity, usually a company, that ows a certain Media. For example Fox Entertainment Group owns the Fox News Channel. Fox Entertainment Group is a NewsProvider. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[NewsProvider](../Submissions/NewsReportingEvent/NewsProvider "Submissions:NewsReportingEvent/NewsProvider") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif "Class") __NewsReportingEvent__ (owl:Class) This is a subclass of ReportingEvent, designed to represent an act of reporting a certain actual event during a news programme or via other news media. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[NewsReportingEvent](../Submissions/NewsReportingEvent/NewsReportingEvent "Submissions:NewsReportingEvent/NewsReportingEvent") page_
[![Class](../images/thumb/2/27/Class.gif/20px-Class.gif)](../Image/Class.gif "Class") __PresentationContext__ (owl:Class) Class for denoting circumstances of an entity presentation. If a waiter presented a dish with an apologetic smile, then the apologetic smile is a PresentationContext. 
 [![](../images/thumb/8/87/ArrowRight.gif/11px-ArrowRight.gif)](../Image/ArrowRight.gif "ArrowRight.gif") _[PresentationContext](../Submissions/NewsReportingEvent/PresentationContext "Submissions:NewsReportingEvent/PresentationContext") page_
#  Additional information


Pattern description is available at: [http://ontologydesignpatterns.org/wiki/Submissions:NewsReportingEvent](../Submissions/NewsReportingEvent "http://ontologydesignpatterns.org/wiki/Submissions:NewsReportingEvent")
Pattern description is included in: E. Kowalczuk, A. Ławrynowicz,



#  Scenarios



__Scenarios about NewsReportingEvent__
No scenario is added to this Content OP.




#  Reviews



__Reviews about NewsReportingEvent__
There is no review about this proposal.
This revision (revision ID __12892__) takes in account the reviews: none


Other info at [evaluation tab](http://ontologydesignpatterns.org/wiki/index.php?title=Submissions:NewsReportingEvent&action=evaluation "http://ontologydesignpatterns.org/wiki/index.php?title=Submissions:NewsReportingEvent&action=evaluation")




  




#  Modeling issues



__Modeling issues about NewsReportingEvent__
There is no Modeling issue related to this proposal.




  




#  References


[Add a reference](index.php@title=Odp%253AAdd_reference&subject=../Submissions/NewsReportingEvent "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_reference&subject=Submissions%3ANewsReportingEvent")


  






Retrieved from "[http://ontologydesignpatterns.org/wiki/Submissions:NewsReportingEvent](../Submissions/NewsReportingEvent)"
 [Categories](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [ProposedContentOP](../Category/ProposedContentOP "Category:ProposedContentOP") | [Submitted to event](../Category/Submitted_to_event "Category:Submitted to event")