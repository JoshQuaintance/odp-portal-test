#  FSDAS Scenario


__Title:__ FSDAS Scenarios


__Description:__ FSDAS simple scenarios for extracting competency questions to be used in the design of the FSDAS application ontology network. 
Formulated by Yves Jaques (UN-FAO). 


__Diagram__
_(this article has no graphical representation)_



#  About


  




#  Additional information


* Species
	+ hasHabitat:str
		- * give me the species having a "demersal" habitat in water area "24" (see [hasHabitat](../Community/HasHabitat "Community:HasHabitat"))
	+ hasSynonyms:str
		- * give me the synonyms and localnames for species "Ostrica gigas"
	+ canBeConfusedWith:species
		- * give me the species with which species "Ostrica gigas" can be confused.
	+ bathymetry:range
		- * give me the species found below 200 metres for water area 24
	+ feedsUpon:Species
		- * give me the species that eat "shrimp"
	+ preyedUponBy:Species\*\*
		- * give me the species eaten by "seals".
	+ caughtByGear:Geartype
		- * give me the species caught using "bottom gillnets"
			* in which water areas are "bottom gillnets" used?
	+ caughtByVessel:Vesseltype
		- * give me the species caught using "gillneters"
			* in which water areas are "gillneters" used?
	+ localNames:str
		- * give me the species containing local name "oyster"
	+ conservationStatus:str
		- * give me the species for which conservation status contains "Vulnerable"


  




* Aquatic Resource
	+ resourceRTMS:int
	+ hasSpecies:Species
		- * Give me the Species for water area 24.
	+ hasWaterArea:WaterArea
		- * Give me the Water areas for species "Gadus morhua"


  




* Aquatic Resource Observation
	+ hasResource:resource
	+ referenceYear:date
		- * Give me the resource observations for the year 2004.
	+ exploitationRate:enum
		- * Give me the resource observations where the exploitation rate is "Moderate fishing mortality"
	+ exploitationState:enum
		- * Give me the resource observations where the state is "fully exploited"
	+ abundanceLevel:enum
		- * Give me the resource observations where the abundance level is "Low abundance"
	+ jurisdictionalDistribution:enum
		- * Give me the resource observations where the jurisdictional distribution is "Highly migratory"
	+ climaticZone:enum
		- * Give me the resource observations where the zone is "Tropical"
	+ verticalDist:enum
		- * Give me the resource observations where the vertical distance (vdist) is "Pelagic"


* Geartype
	+ targetSpecies:Species
		- * Give me the gears targeting species "tuna"
	+ incidentalSpecies:Species
		- * Give me the gears which incidentally catch species "dolphins"


* Vesseltype
	+ usesGeartype:Geartype
		- * Give me the vesseltypes that use "trawls"


#  References


[Add a reference](index.php@title=Odp%253AAdd_reference&subject=Community%253AFSDAS+Scenario.html "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_reference&subject=Community%3AFSDAS+Scenario")


  




 [List of Modeling Issues](../Community/Main "Community:Main") | [Post a new modeling issue](../Community/PostModelingIssue "Community:PostModelingIssue") | [Add a comment in the discussion page](index.php@title=Odp%253AAdd_comment&target=Community_talk%253AFSDAS_Scenario.html#New_comment "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_comment&target=Community_talk:FSDAS_Scenario#New_comment")


Retrieved from "[http://ontologydesignpatterns.org/wiki/Community:FSDAS\_Scenario](../Community/FSDAS_Scenario)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [ModelingIssue](../Category/ModelingIssue "Category:ModelingIssue")