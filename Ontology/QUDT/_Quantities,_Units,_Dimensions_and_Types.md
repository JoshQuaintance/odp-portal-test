Return to [Catalogue of Exemplary Ontologies](../../Ontology/Main.md "Ontology:Main")



#  Ontology Overview


#  Long Description


The QUDT ontologies provide the following:



1. Multiple Systems of Units
2. Comprehensive Coverage of Quantities
3. Ontology Support for Units Conversion using Dimensions
4. Simple and Structured Data Types


###   Quantities, Quantity Kinds, and Quantity Values


A __Quantity__ is an observable property of an object, event or system that can be measured and quantified numerically. Quantities are differentiated by two attributes which together comprise the essential parameters needed to formalize the structure of quantities: kind and magnitude. The kind attribute of a quantity identifies the observable property quantified, e.g. length, force, frequency; the magnitude of the quantity expresses its relative size compared to other quantities of the same kind.


For example, the speed of light in a vacuum and the escape velocity of the Earth are both quantities of the kind speed but are of different magnitudes. The speed of light in a vacuum is greater than the escape velocity of the Earth. More generally, the speed of light in a vacuum is comparable to the escape velocity of the Earth. Thus, if two quantities of the same kind, their magnitudes can be compared and ordered. However, the same is not true if the quantities are of different kinds. There is no intrinsic way to compare the magnitude of a quantity of mass with the magnitude of a quantity of length.


Quantities may arise from definition or convention, or they may be the result of one or a series of experiments and measurements. In the first case, the quantity is _exact_; in the second case, measurement uncertainty cannot be discounted so the expression of a quantity's magnitude must account for the parameters of uncertainty.



###   Quantity Kinds


A __Quantity Kind__ is any observable property that can be measured and quantified numerically. Familiar examples include physical properties such as length, mass, time, force, energy, power, electric charge, etc. Less familiar examples include currency, interest rate, price to earning ratio, and information capacity.



###   Unit of Measure


A __Unit of Measure__ or __Unit__ is a particular quantity of a given kind that has been chosen as a scale for measuring other quantities of the same kind. For example, the Meter is a quantity of length that has been empirically defined by the BIPM. Any quantity of length can be expressed as a number multiplied by the unit meter.


More formally, the value of a quantity Q with respect to a unit (U) is expressed as the scalar multiple of a real number (n) and U:


Q = nU



###   Quantity Value


A quantity value expresses the numerical value of a quantity with respect to a chosen unit of measure. For example, the value of Planck's constant in Joule-Seconds (J s) is approximately 6.62606896E-34, whereas the value in Erg-Seconds (erg s) is approximately 6.62606896E-27.


The OWL model for the classes qud:QuantityKind, qud:Quantity, qud:QuantityValue, qud:Unit is shown below.


  




###   Systems of Quantities and Units


The art and science of defining, standardizing, and organizing quantity kinds and units is ancient and modern. Today, scientific boards and standards bodies maintain rigorous definitions for quantity kinds and units. The definitions of and relationships between quantity kinds are derived from physical laws and mathematical transformations. Units are defined by experimental observations, by the application of physical laws, as ratios of fundamental physical constants, or by reference. One significant advance in the modern treatment of metrology has been the use of logic and mathematics to organize quantity kinds and units into systems and to analyze the relationships between them.


A system of quantity kinds is a set of one or more quantity kinds together with a set of zero or more algebraic equations that define relationships between quantity kinds in the set. In the physical sciences, the equations relating quantity kinds are typically physical laws and definitional relations, and constants of proportionality. Examples include Newton’s First Law of Motion, Coulomb’s Law, and the definition of velocity as the instantaneous change in position.


In almost all cases, the system identifies a subset of base quantity kinds. The base set is chosen so that all other quantity kinds of interest can be derived from the base quantity kinds and the algebraic equations.


A system of units is a set of units which are chosen as the reference scales for some set of quantity kinds together with the definitions of each unit. Units may be defined by experimental observation or by proportion to another unit not included in the system. If the unit system is explicitly associated with a quantity kind system, then the unit system must define at least one unit for each quantity kind.



###   Base and Derived Quantity Kinds


Many systems of quantity kinds identify a special subset of the included quantity kinds called the base quantity kinds. Base quantity kinds are typically chosen so that no base quantity kind can be expressed as an algebraic relation of one or more other base quantity kinds using only the constituent equations included in the system. A quantity kind that can be expressed as an algebraic relation of one or more base quantity kind is called a derived quantity kind. Thus, in any quantity kind system, the base set and derived set are disjoint.


Similarly, unit systems may distinguish between base units and derived units. A base unit is a unit of measurement for a base quantity, and a derived unit is a unit of measurement for a derived quantity. Unit systems define at least one base unit for each base quantity and at least one derived unit for each derived quantity.



###   Quantity Dimensions


Quantity kind systems that define base and derived sets have certain mathematical properties that permit quantity kinds to be manipulated symbolically. The construction goes as follows: Assign a distinct dimension symbol to each base quantity kind. For each derived quantity kind, take the formula that expresses it in terms of the base quantity kinds and replace every occurrence of a base quantity with its symbol. This is the dimension symbol for the derived quantity kind. In this way, every quantity kind maps to a dimension symbol of the form:


dim Q = (B1)d1(B2)d2…(Bn)dn


Here {B1,…,Bn} are the dimension symbols for the base quantities and {d1,…,dn} are rational numbers. Typically, the values of the di are between -3 and 3, however magnitudes as high as 7 are required to cover the range of quantity kinds currently defined. Using the multiplication identity for exponents AnAm = An+m one can show that the set of dimension symbols is homomorphic to an n-dimensional vector space over the rational numbers. Multiplication of quantity kinds corresponds to vector addition, division corresponds to vector subtraction, and inverting a quantity kind corresponds to computing the additive inverse of its dimension vector.


In some cases, distinct quantity kinds may have the same dimension symbol. This often occurs in cases where physical laws are discovered and formalized independently of each other, but reduce to the same base quantity kinds. Perhaps the most commonly quoted example is the dimensional equivalence of mechanical torque and energy. Both have the same dimensions (L2MT-2) but are defined very differently. One consequence of the equivalence is that the same units of measure are applicable to both. One salient difference between the two in this example is that torque is a pseudo-vector while energy is a scalar. However, this distinction (value type) is not accounted for in the quantity kind system formalism.



#  Additional Information


  



  




#  References


[Add a reference](index.php@title=Odp%253AAdd_reference&subject=Ontology%253AQUDT%253A+Quantities,+Units,+Dimensions+and+Types.html "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_reference&subject=Ontology%3AQUDT%3A+Quantities%2C+Units%2C+Dimensions+and+Types")



* QUDT home page [Project Home Page](http://www.oegov.us/blog/?page_id=109 "http://www.oegov.us/blog/?page_id=109") | [reference page](../../Community/References/QUDT_home_page.md "Community:References/QUDT home page")




Retrieved from "[http://ontologydesignpatterns.org/wiki/Ontology:QUDT:\_Quantities%2C\_Units%2C\_Dimensions\_and\_Types](../../Ontology/QUDT/_Quantities,_Units,_Dimensions_and_Types.md)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [Ontology](../../Category/Ontology.md "Category:Ontology")