##   XD with the NeOn toolkit


Below you find some hints on how to use the XD plugin.



* You need an Internet connection to use the XD plugin.
* To find the XD perspective in the toolkit, in the menus choose Window->Open perspective->Other... Then select "eXtreme Design" in the list of perspectives. It will take some minutes to open because it creates a cache of all the patterns from the portal.
* At the bottom left you have a panel showing two tabs: "ODP registry" and "ODP selections". The registry is the list of patterns in the portal, you find them under the folder "Submissions".
* If you mark a pattern in the list the information about the pattern will appear in the pane to the right. This is the same information as in the portal, but without the graphical visualization.
* If you want to reuse a pattern you have two options: "getting" it to your workspace or directly specializing it.
	+ "Get" can be found as a button above the bottom left tabs, it shows a green arrow. Get means "copy the pattern owl-file into my workspace directory so that I can use it later". If you then go back to the NTK perspective you can for example import this like any other ontology, or open it to visualize it etc. Most likely you would now import the pattern file into your ontology, and then start specializing the classes and properties of the pattern, all of this using the "normal" NTK perspective that you are used to already.
	+ "Specialize" can be found as a button next to the "get" one, but with a blue arrow. Specialize in this case means "help me to specialize the pattern using a wizard". This opens a wizard that step by step takes you through the same process as when you specialize a pattern "without guidance", i.e. the result will be exactly the same as if you get the pattern, import it, specialize all the classes and properties in the NTK perspective, the difference is only in the interface and the guidance of the process.
* If you don't find the pattern you need there is also a simple search functionality. It is under the tab "ODP selections". Here you can click the button "simple search" and do a keyword search over the patterns. This can be useful if you for example remember from the lecture that there should be something called situation, but you cannot find it. The result is presented in two lists, the first is showing a classical keyword search and the second shows an expanded search where things like synonyms and related terms have been taken into account. When selecting a search result you can do the same operations, get or specialize, as above.


  

__Specialization wizard__


When using the specialization wizard you will first be asked what you want the result to be, i.e. if you want to create a new ontology containing the specialized pattern, and if you want to import it into another ontology in your workspace or if you want to keep it separate for now. Depending on what you choose you have to also give the new ontology a URI and possibly select where to import it or where to put it in your workspace. 


Next, you should select the parts of the pattern that you want to specialize (sometimes maybe you are not interested in using all the pattern). After this you will be asked to add the specializations of the selected classes and properties: mark an element and click on "add specialization" to the right. Now you have to give a new name to your specific class/property, then add a label, and then a comment. The wizard forces you to use good practices, i.e. to add labels and comments. Don't forget to click on "add" every time you finish writing something. If you are specializing a property you will automatically be forced to specialize also its inverse. 


When you have specialized all the things you selected before, you can go on to the next step. Here you will be shown the restrictions that may hold for each of the new classes and properties. They are stated in natural language, but represent for example domain and range restrictions, disjointness etc. Mark all the statements that hold for your ontology. Consider that you should be as specific as possible, i.e. prefer statements that include your specific classes rather than general ones nvolving the pattern classes and properties. 


When you select "next", you get a summary of what you have created. If it looks ok, then proceed. Finally you get a question if you want to annotate the module you have created. In this case an annotation wizard opens, where you can add comments and other annotations to describe your new ontology.





Retrieved from "[http://ontologydesignpatterns.org/wiki/Training:Autumn\_2009\_-\_ODPs%40UPM/XD-help](../../Training/Autumn_2009_-_ODPs@UPM/XD-help.md)"