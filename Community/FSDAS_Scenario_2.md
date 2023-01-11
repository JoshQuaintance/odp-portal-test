#  FSDAS Scenario 2


__Title:__ FSDAS Scenario 2


__Description:__ Massaged scenarios based on modeling issues Community:FSDAS Scenario]] 


__Diagram__
_(this article has no graphical representation)_



#  About


  




#  Additional information


__Diagram__
_(this article has no graphical representation)_


  




##   Scenarios and associated solutions


The following scenarios contain no additional hints for modeling. For a version with hints, see also the [original modeling issue](../Community/FSDAS_Scenario.md "Community:FSDAS Scenario") from Yves. The link on the right of leading scenarios refers to the OWL file of a content pattern that is proposed to satisfy the scenario:



1. give me the species containing local name "oyster" [current content pattern](http://www.ontologydesignpatterns.org/cp/owl/fsdas/speciesnames.owl "http://www.ontologydesignpatterns.org/cp/owl/fsdas/speciesnames.owl")
	1. give me the synonyms and localnames for species "Ostrica gigas"
	2. give me the species with which species "Ostrica gigas" can be confused
2. give me the Species for water area "24" [current content pattern](http://www.ontologydesignpatterns.org/cp/owl/fsdas/aquaticresources.owl "http://www.ontologydesignpatterns.org/cp/owl/fsdas/aquaticresources.owl")
	1. give me the Water areas for species "Gadus morhua"
3. give me the species having a "demersal" habitat in water area "24" [current content pattern](http://www.ontologydesignpatterns.org/cp/owl/fsdas/specieshabitat.owl "http://www.ontologydesignpatterns.org/cp/owl/fsdas/specieshabitat.owl")
4. give me the species found below 200 metres for water area "24" [current content pattern](http://www.ontologydesignpatterns.org/cp/owl/fsdas/speciesbathymetry.owl "http://www.ontologydesignpatterns.org/cp/owl/fsdas/speciesbathymetry.owl"), an alternate pattern (deprecated by fishery experts, which seem to assume a fixed value for a species' bathymetric range) for habitat and bathymetric range within one specific water area, based on the situation pattern, is [here](http://www.ontologydesignpatterns.org/cp/owl/fsdas/speciesconditions.owl "http://www.ontologydesignpatterns.org/cp/owl/fsdas/speciesconditions.owl")
5. give me the species that eat "shrimp" [current content pattern](http://www.ontologydesignpatterns.org/cp/owl/fsdas/specieseat.owl "http://www.ontologydesignpatterns.org/cp/owl/fsdas/specieseat.owl")
	1. give me the species eaten by "seals"
6. give me the resource observations for the year 2004 [current content pattern](http://www.ontologydesignpatterns.org/cp/owl/fsdas/aquaticresourceobservation.owl "http://www.ontologydesignpatterns.org/cp/owl/fsdas/aquaticresourceobservation.owl"). This is now deprecated by fishery experts, who seem to assume 'fixed' values for some of the observations. In the following, the observation scenarios are arranged into two patterns (one for 1-2 and one for 3), while those having fixed values are arranged into three scenarios (one each for 4, 5, and 6):
7. give me the resource observations where the exploitation rate is "Moderate fishing mortality" [current content pattern](http://www.ontologydesignpatterns.org/cp/owl/fsdas/resourceexploitationobservation.owl "http://www.ontologydesignpatterns.org/cp/owl/fsdas/resourceexploitationobservation.owl")
	1. give me the resource observations where the state is "fully exploited"
8. give me the resource observations where the abundance level is "Low abundance" [current content pattern](http://www.ontologydesignpatterns.org/cp/owl/fsdas/resourceabundancenobservation.owl "http://www.ontologydesignpatterns.org/cp/owl/fsdas/resourceabundancenobservation.owl")
9. give me the resource observations where the jurisdictional distribution is "Highly migratory" [current content pattern](http://www.ontologydesignpatterns.org/cp/owl/fsdas/jurisdictionaldistribution.owl "http://www.ontologydesignpatterns.org/cp/owl/fsdas/jurisdictionaldistribution.owl")
10. give me the resource observations where the climatic zone is "Tropical" [current content pattern](http://www.ontologydesignpatterns.org/cp/owl/fsdas/climaticzone.owl "http://www.ontologydesignpatterns.org/cp/owl/fsdas/climaticzone.owl")
11. give me the resource observations where the vertical distance (vdist) is "Pelagic" [current content pattern](http://www.ontologydesignpatterns.org/cp/owl/fsdas/verticaldistance.owl "http://www.ontologydesignpatterns.org/cp/owl/fsdas/verticaldistance.owl")
12. give me the species for which conservation status contains "Vulnerable" [current content pattern](http://www.ontologydesignpatterns.org/cp/owl/fsdas/speciesconservation.owl "http://www.ontologydesignpatterns.org/cp/owl/fsdas/speciesconservation.owl")
13. give me the gears targeting species "tuna" [current content pattern](http://www.ontologydesignpatterns.org/cp/owl/fsdas/gearspecies.owl "http://www.ontologydesignpatterns.org/cp/owl/fsdas/gearspecies.owl")
	1. give me the gears which incidentally catch species "dolphins"
	2. give me the species caught using "bottom gillnets"
14. in which water areas are "bottom gillnets" used? [current content pattern](http://www.ontologydesignpatterns.org/cp/owl/fsdas/gearwaterarea.owl "http://www.ontologydesignpatterns.org/cp/owl/fsdas/gearwaterarea.owl")
15. give me the species caught using "gillneters" [current content pattern](http://www.ontologydesignpatterns.org/cp/owl/fsdas/vesselspecies.owl "http://www.ontologydesignpatterns.org/cp/owl/fsdas/vesselspecies.owl")
16. in which water areas are "gillneters" used? [current content pattern](http://www.ontologydesignpatterns.org/cp/owl/fsdas/vesselwaterarea.owl "http://www.ontologydesignpatterns.org/cp/owl/fsdas/vesselwaterarea.owl")
17. give me the vesseltypes that use "trawls" [current content pattern](http://www.ontologydesignpatterns.org/cp/owl/fsdas/gearvessel.owl "http://www.ontologydesignpatterns.org/cp/owl/fsdas/gearvessel.owl")


##   Scenarios abstracted as competency questions (with associated solutions)


The following competency questions contain no additional hints for modeling. For a version with hints, see also the [original modeling issue](../Community/FSDAS_Scenario.md "Community:FSDAS Scenario") from Yves. The link on the right of leading competency questions refers to the OWL file of a content pattern that is proposed to satisfy the competency questions:



1. what species contain a certain local name? [current content pattern](http://www.ontologydesignpatterns.org/cp/owl/fsdas/speciesnames.owl "http://www.ontologydesignpatterns.org/cp/owl/fsdas/speciesnames.owl")
	1. what are synonyms and localnames for a certain species?
	2. what are the species with which a certain species can be confused?
2. what are the species for a certain water area? [current content pattern](http://www.ontologydesignpatterns.org/cp/owl/fsdas/aquaticresources.owl "http://www.ontologydesignpatterns.org/cp/owl/fsdas/aquaticresources.owl")
	1. what are the water areas for a species?
3. what are the species having a certain habitat in a water area? [current content pattern](http://www.ontologydesignpatterns.org/cp/owl/fsdas/specieshabitat.owl "http://www.ontologydesignpatterns.org/cp/owl/fsdas/specieshabitat.owl")
4. what are the species found at a certain bathymetric range for a water area? [current content pattern](http://www.ontologydesignpatterns.org/cp/owl/fsdas/speciesbathymetry.owl "http://www.ontologydesignpatterns.org/cp/owl/fsdas/speciesbathymetry.owl"), an alternate pattern (deprecated by fishery experts, which seem to assume a fixed value for a species' bathymetric range) for habitat and bathymetric range within one specific water area, based on the situation pattern, is [here](http://www.ontologydesignpatterns.org/cp/owl/fsdas/speciesconditions.owl "http://www.ontologydesignpatterns.org/cp/owl/fsdas/speciesconditions.owl")
5. what are the species that eat a certain species? [current content pattern](http://www.ontologydesignpatterns.org/cp/owl/fsdas/specieseat.owl "http://www.ontologydesignpatterns.org/cp/owl/fsdas/specieseat.owl")
	1. what are the species eaten by another species?
6. what are the resource observations for a certain year? [current content pattern](http://www.ontologydesignpatterns.org/cp/owl/fsdas/aquaticresourceobservation.owl "http://www.ontologydesignpatterns.org/cp/owl/fsdas/aquaticresourceobservation.owl"). This is now deprecated by fishery experts, who seem to assume 'fixed' values for some of the observations. In the following, the observation scenarios are arranged into two patterns (one for 1-2 and one for 3), while those having fixed values are arranged into three scenarios (one each for 4, 5, and 6):
7. what are the resource observations with a certain the exploitation rate? [current content pattern](http://www.ontologydesignpatterns.org/cp/owl/fsdas/resourceexploitationobservation.owl "http://www.ontologydesignpatterns.org/cp/owl/fsdas/resourceexploitationobservation.owl")
	1. what are the resource observations with a certain exploitation state?
8. what are the resource observations with a certain abundance level? [current content pattern](http://www.ontologydesignpatterns.org/cp/owl/fsdas/resourceabundancenobservation.owl "http://www.ontologydesignpatterns.org/cp/owl/fsdas/resourceabundancenobservation.owl")
9. what are the resource observations with a certain jurisdictional distribution? [current content pattern](http://www.ontologydesignpatterns.org/cp/owl/fsdas/jurisdictionaldistribution.owl "http://www.ontologydesignpatterns.org/cp/owl/fsdas/jurisdictionaldistribution.owl")
10. what are the resource observations with a certain climatic zone? [current content pattern](http://www.ontologydesignpatterns.org/cp/owl/fsdas/climaticzone.owl "http://www.ontologydesignpatterns.org/cp/owl/fsdas/climaticzone.owl")
11. what are the resource observations with a certain vertical distance? [current content pattern](http://www.ontologydesignpatterns.org/cp/owl/fsdas/verticaldistance.owl "http://www.ontologydesignpatterns.org/cp/owl/fsdas/verticaldistance.owl")
12. what are the species with a certain conservation status? [current content pattern](http://www.ontologydesignpatterns.org/cp/owl/fsdas/speciesconservation.owl "http://www.ontologydesignpatterns.org/cp/owl/fsdas/speciesconservation.owl")
13. what are the gear types targeting a species? [current content pattern](http://www.ontologydesignpatterns.org/cp/owl/fsdas/gearspecies.owl "http://www.ontologydesignpatterns.org/cp/owl/fsdas/gearspecies.owl")
	1. what are the gear types which incidentally catch other species?
	2. what are the species caught using a gear type?
14. in which water areas is a gear type used? [current content pattern](http://www.ontologydesignpatterns.org/cp/owl/fsdas/gearwaterarea.owl "http://www.ontologydesignpatterns.org/cp/owl/fsdas/gearwaterarea.owl")
15. what are the species caught using a vessel type? [current content pattern](http://www.ontologydesignpatterns.org/cp/owl/fsdas/vesselspecies.owl "http://www.ontologydesignpatterns.org/cp/owl/fsdas/vesselspecies.owl")
16. in which water areas is a vessel type used? [current content pattern](http://www.ontologydesignpatterns.org/cp/owl/fsdas/vesselwaterarea.owl "http://www.ontologydesignpatterns.org/cp/owl/fsdas/vesselwaterarea.owl")
17. what are the vessel types that use a gear type? [current content pattern](http://www.ontologydesignpatterns.org/cp/owl/fsdas/gearvessel.owl "http://www.ontologydesignpatterns.org/cp/owl/fsdas/gearvessel.owl")


#  References


[Add a reference](index.php@title=Odp%253AAdd_reference&subject=Community%253AFSDAS+Scenario+2.html "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_reference&subject=Community%3AFSDAS+Scenario+2")


  






Retrieved from "[http://ontologydesignpatterns.org/wiki/Community:FSDAS\_Scenario\_2](../Community/FSDAS_Scenario_2.md)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [ModelingIssue](../Category/ModelingIssue.md "Category:ModelingIssue")