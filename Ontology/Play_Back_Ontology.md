Return to [Catalogue of Exemplary Ontologies](../Ontology/Main.md "Ontology:Main")



#  Ontology Overview


#  Long Description


The Play Back Ontology provides basic concepts and properties for describing concepts that are related to the play back domain, e.g. a playlist, play back and skip counter, on/ for the Semantic Web.




```
   The play back domain could be seen as a subset of the media domain - it deals with playing back some media, e.g. videos, music tracks or slideshows, somehow.

```

On the basis of this definition the objects that are included into this domain are media objects. That means all concepts of the Play Back Ontology are somehow related to at least one media object. The range of these media objects is currently restricted to the concepts bibo:Document and frbr:Endeavour, incl. all their sub classes, e.g. mo:Track.
The pbo:Playlist concept is a sub class of olo:OrderedList and hence, a specialized ordered list of the media domain. Therefore, a pbo:Playlist instance consists of pbo:PlaylistSlot instances (related by pbo:playlist\_slot), which are related to at least one media item by using the property pbo:playlist\_item. pbo:Playlist has a further sub class, pbo:FixedPlaylist, to described playlists or sections of playlists, which have a strict order, e.g. a section of music tracks that should be played always one after another, or that are somehow related to each other. Furthermore, pbo:Playlist instances can be related to something by using the property pbo:playlist.
The Play Back Ontology consists further more of a couple of media action counters, which are represented by pbo:MediaActionCounter. Sub classes of this concept are pbo:PlayBackCounter and pbo:SkipCounter. Due to the property pbo:media\_object, which is a sub property of co:object, it is possible to only associate media objects to pbo:MediaActionCounter instances.
The Play Back Ontology and the illustrated examples above demonstrates the reutilization, specialization and application of concepts of existing ontologies (Ordered List Ontology, Counter Ontology, Association Ontology, Music Ontology, Similarity Ontology, DCMI Metadata Terms, ...). Please feel free to create further, more specialized concepts and properties, which are based on the introduced ontologies, e.g. describing transition of music tracks in dj mixes (as discussed here).



#  Additional Information


  



  




#  References


[Add a reference](index.php@title=Odp%253AAdd_reference&subject=Ontology%253APlay+Back+Ontology.html "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_reference&subject=Ontology%3APlay+Back+Ontology")



* A blog post about the Recommendation Ontology with examples and graphics. [Weblog post](http://smiy.org/2010/07/27/the-play-back-ontology/ "http://smiy.org/2010/07/27/the-play-back-ontology/") | [reference page](../Community/References/Play_Back_Ontology_announcement.md "Community:References/Play Back Ontology announcement")




Retrieved from "[http://ontologydesignpatterns.org/wiki/Ontology:Play\_Back\_Ontology](../Ontology/Play_Back_Ontology.md)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [Ontology](../Category/Ontology.md "Category:Ontology")