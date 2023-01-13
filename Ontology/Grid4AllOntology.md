Return to [Catalogue of Exemplary Ontologies](../Ontology/Main "Ontology:Main")



#  Ontology Overview


#  Long Description


The Semantic Information System (SIS) provides a matching and selection service between peers (humans or software agents) that offer or request (place any of the two kinds of orders i.e. either offers or requests) resources and services within grid environments. This service is used by the Grid4All market place. In the market place, resource/service consumers and providers negotiate traded entities in auction based markets, where these markets are spontaneously initiated (instantiated) by different actors, such as resource/services providers, consumers, or 3rd party actors. Markets are accessed as services that are themselves advertised at the Semantic Information System. 


SIS acts as a registry for the following types of services: Markets, Application Services and Services exposing resources. The SIS may be queried by software agents as well as by human users to select advertised services and resources: Matchmaking happens through different criteria concerning resources and other application specific traded domain entities, as well as services' profiles. The returned query results are ranked according to resources/services matching characteristics and providers'/consumers' features. 


The matchmaking process is executed in the following cases:


A user makes a request, in which case provider-initiated markets offering services/resources are returned
A user makes an offer, in which case consumer-initiated markets are returned.


After the matchmaking is completed, and a set of results is obtained, there is an additional step prior to their presentation: the ranking process. Matchmaking performs a coarse-grained distinction of results, according to the type of match ("exact" and "subsumes" match). The ranking process provides an ordering of results which reflects the preferences of the user (e.g. preference on specific peers). It should be noted that the ranking process is implemented as a component of SIS, i.e. the Selection component. Finally, the list of results is returned to the user. According to what specifications have been given as input to the system, a list of resources/services may be returned or the list of the corresponding markets.



#  Additional Information


  



  




#  References


[Add a reference](index.php@title=Odp%253AAdd_reference&subject=../Ontology/Grid4AllOntology "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_reference&subject=Ontology%3AGrid4AllOntology")



* Vouros, G., A. Papasalouros, K. Kotis, A. Valarakos, and K. Tzonas, "The Grid4All ontology for the retrieval of traded resources in a market-oriented Grid", IJWGS special issue on Web/Grid Information and Services Discovery and Management, vol. 4, pp. 418-439, 00/2008. [Paper](http://www.icsd.aegean.gr/kotis/publications/IJWGS.pdf "http://www.icsd.aegean.gr/kotis/publications/IJWGS.pdf") | [reference page](../Community/References/IJWGS_Paper "Community:References/IJWGS Paper")




Retrieved from "[http://ontologydesignpatterns.org/wiki/Ontology:Grid4AllOntology](../Ontology/Grid4AllOntology)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [Ontology](../Category/Ontology "Category:Ontology")