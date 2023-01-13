Return to [Catalogue of Exemplary Ontologies](../Ontology/Main "Ontology:Main")



#  Ontology Overview


#  Long Description


#  Additional Information


  

SRE - Sub-pixel Efficacy Region & SRI - Signal Resilient to Interpolation:
ONTOLOGY, made by Carlo Ciulla (carlo.ciulla@UIST.edu.mk, cxc2728@NJIT.edu)


SRE – Sub-pixel Efficacy Region: Spatial region of points where the first order derivative of the intensity-curvature functional is zero. 


SRE-based interpolation functions: Interpolation functions derived from the Sub-pixel Efficacy Region, which normally may display improved approximation characteristics than the classic interpolation functions from which they are derived from. The improved approximation characteristics are manifest with a lower interpolation error.


Novel Re-sampling Locations: Re-sampling locations where the SRE-based interpolation function displays improved approximation characteristics than the classic interpolation functions from which they are derived from.


Classic curvature: Sum of all of the second order derivatives of the interpolation function. The classic curvature is employed to calculate the Pixel-Intensity Correction (PIC) using the interpolation function.


Classic-curvature interpolation formula: The interpolation formula made of the sum of: the numerical value of the pixel to re-sample and the Pixel-Intensity Correction (PIC). The Classic-curvature interpolation formula is calculated using the classic-curvature of the interpolation function.


C.RC ratio of improvement: Is the ratio indicating the relativity of performance between the classic-resilient-curvature (hybrid) formula and the classic-curvature interpolation formula. It is calculated as percentage value of the ratio between the MAE of the classic-curvature interpolation formula and the MAE of the hybrid formula, with the math expression: (1.0 - (MAE of the classic-curvature interpolation formula / MAE of the hybrid formula)).


Classic-resilient-curvature interpolation formula (hybrid formula): The formula which combines the two formulae (classic-curvature and resilient-curvature) depending on which one of the two gives lowest Mean Absolute Error (MAE). The concept applies on a node-to-node basis (in 1D), and on a pixel-to-pixel basis (in 2D), and on a voxel-to-voxel basis (in 3D). The hybrid formula is employed to improve the performance of both classic-curvature formula and resilient-curvature formula.


Classic Signal: The signal in its original form as modeled through an interpolation function without any processing. The interpolation function is any of those treated in this book (e.g. bivariate quadratic B-Spline interpolation function, trivariate cubic B-Spline, etc.).


Intensity-curvature multiplication: In 1D is the term comprising of the multiplication between the node intensity (f(0)) and the second order derivative. In 2D and 3D, the intensity-curvature multiplication is the multiplication between the pixel intensity (f(0, 0)) and the sum of second order derivatives calculated respect to the dimensional variables. The intensity-curvature multiplication is employed to measure the combined information content of both pixel intensity and curvature of the interpolation function. This concept was initially introduced in: Ciulla & Deek (2005).


Intensity-curvature term before interpolation (Eo): Is the integral of the intensity-curvature multiplication calculated: inside the closed interval [0, x] in 1D, inside the closed interval [(0, 0), (x, y)] in 2D, inside the closed interval [(0, 0, 0), (x, y, z)] in 3D. In 1D the intensity-curvature multiplication is calculated through the multiplication between the sampled intensity value and the second order derivative. In 2D and 3D, the intensity-curvature multiplication is calculated through the multiplication between the sampled intensity value and the sum of second order derivatives calculated respect to the dimensional variables. The second order derivatives are calculated at the node (in 1D) or grid point (in 2D or 3D). The intensity-curvature term before interpolation (Ciulla, (2009)) is employed to measure the energy level of the non-interpolated signal (for given interpolation function). 


A note to the reader is due. There is a difference between the intensity-curvature term before interpolation calculated in Ciulla , (2012) and the intensity-curvature term before interpolation reported in Ciulla, (2009). The difference is that in: Ciulla, (2009), the second order derivatives employed to calculate (Eo) are 3 in the covariates in 3D, are 2 in the covariates in 2D, and 1 in the univariate in 1D.


Intensity-curvature term after interpolation (EIN): Is the integral of the intensity-curvature multiplication calculated: inside the closed interval [0, x] in 1D, inside the closed interval [(0, 0), (x, y)] in 2D, inside the closed interval [(0, 0, 0), (x, y, z)] in 3D. In 1D the intensity-curvature multiplication is calculated at the intra-nodal point x through the multiplication between the intensity value given by the interpolation function and the second order derivative. In 2D and 3D the intensity-curvature multiplication is calculated at the grid location (x, y) through the multiplication between the intensity value given by the interpolation function and the sum of second order derivatives respect to the dimensional variables. The second order derivatives are calculated at the intra-nodal (1D) or intra-pixel (2D), or intra-voxel (3D) point identified with x in 1D, identified with (x, y) in 2D, identified with (x, y z) in 3D. The intensity-curvature functional after interpolation (Ciulla, (2009)) is employed to measure the energy level of the interpolated signal (for given interpolation function). 


A note to the reader is due. There is a difference between the intensity-curvature term after interpolation calculated in Ciulla, (2012) and the intensity-curvature term before interpolation reported in Ciulla, (2009). The difference is that in: Ciulla, (2009), the second order derivatives employed to calculate (Eo) are 3 in the covariates in 3D, are 2 in the covariates in 2D, and 1 in the univariate in 1D.


Intensity-Curvature Functional: The ratio between two intensity-curvature terms before (Eo) and after (EIN) interpolation, which is: Eo/EIN. The Intensity-Curvature Functional (Ciulla, 2009) is employed to measure the energy level change determined through the interpolation function. 


Mean Absolute Error (MAE): The absolute value of the difference between the value of the signal and the interpolated signal. The MAE can be calculated at a given node (in 1D), or pixel (in 2D), or voxel (in 3D). The MAE can be calculated for the classic-curvature interpolation formula, the resilient-curvature interpolation formula, and the classic-resilient-curvature interpolation formula (hybrid formula). The MAE is employed to seek for energy preservation (quest for minimal energy state).


Pixel-Intensity Correction (PIC): The fraction of pixel intensity employed to calculate the signal at a given location not sampled through the sampling device. The PIC is computed through the product between the misplacement and the trigonometric tangent function of the total curvature (which is defined as the sum of all of second order derivatives) of the interpolation function. The PIC can be calculated using either classic curvature or resilient curvature. The Pixel-Intensity-Correction (PIC) acts as the transfer function obtained from the math form of the interpolation function.


Ratio of improvement: Generally, (i) the more negative the ratio of improvement is, the better is the improvement of one interpolation formula over the another interpolation formula; or (ii) the more negative the ratio of improvement is, the more effective the gain in merging one interpolation formula (for instance the classic-curvature interpolation formula) with another interpolation formula (for instance the resilient-curvature interpolation formula) on a pixel-by-pixel basis is, and the higher the gain of the resulting interpolation formula which transforms itself into the resulting interpolation formula (for instance the classic-resilient-curvature interpolation formula (or so called hybrid formula)).


(i) For instance negative values of the ratio of improvement are indicative of superiority in signal reconstruction of resilient interpolation over classic interpolation (Newton & Huygens, trans. 1934), whereas positive values of the ratio of improvement are indicative of superiority in signal reconstruction of classic interpolation over resilient interpolation. The ratio of improvement is calculated with the math expression: (1.0 - (MAE of classic interpolation / MAE of resilient interpolation)) when measuring the relativity of performance between classic interpolation and resilient interpolation. 


(ii) For instance merging the classic-curvature interpolation formula and the resilient-curvature interpolation formula on a pixel-by-pixel basis entails a gain visible through the classic-resilient-curvature interpolation formula (or so called hybrid formula). Such gain can be measured through the C.RC ratio of improvement with the math expression: (1.0 - (MAE of the classic-curvature interpolation formula / MAE of the hybrid formula)), or through the R.CR ratio of improvement with the math expression: (1.0 - (MAE of the resilient-curvature interpolation formula / MAE of the hybrid formula)).


R.CR ratio of improvement: Is the ratio indicating the relativity of performance between the classic-resilient-curvature (hybrid) formula and the resilient-curvature interpolation formula. It is calculated as percentage value of the ratio between the MAE of the resilient-curvature interpolation formula and the MAE of the hybrid formula, with the math expression: (1.0 - (MAE of the resilient-curvature interpolation formula / MAE of the hybrid formula)).


Resilient curvature: Sum of all of the second order derivatives of the Signal Resilient to Interpolation (SRI) derived from the interpolation function. The resilient curvature is employed to calculate the Pixel-Intensity Correction (PIC) using the Signal Resilient to Interpolation (SRI) derived from the interpolation function.


Resilient-curvature interpolation formula: The interpolation formula made of the sum of: the numerical value of the pixel to re-sample and the Pixel-Intensity Correction (PIC). The Resilient-curvature interpolation formula is calculated using the resilient-curvature of the interpolation function.


Resilient interpolation: The concept resilient interpolation is closely linked to that of the equation between the intensity curvature terms before (no interpolation) and after interpolation (see chapter 1). The term resilient interpolation is also used in the book as acronym of Resilient-curvature interpolation formula. The term resilient interpolation is used in chapter 4, whereas the term Resilient-curvature interpolation formula is used in chapters 8 and 12. Both of the terms are related to the formula used to re-sample the signal, which is: the sum of the numerical value of the pixel to re-sample and the Pixel-Intensity Correction (PIC). Whereas in chapter 4 and 8 the aforementioned formula is used in 2D, in chapter 12 the formula is used in 1D, 2D and 3D.


Signal Resilient to Interpolation (SRI): The signal obtained through the solution of the equation of the two intensity-curvature terms before (Eo) and after (EIN) interpolation. The SRI is derived univocally on the basis of a given interpolation function. The SRI is employed to obtain the Resilient-curvature interpolation formula.


Total curvature of an interpolation function: Is defined to be the sum of second order derivatives of the math form of the interpolation function respect to the dimensional variables. 


  

Total curvature of the Signal Resilient to Interpolation: Is defined to be the sum of second order derivatives of the math form of the Signal Resilient to Interpolation (SRI) respect to the dimensional variables. 


  

Virtual shift-rotation: In 1D, a signal is virtually shifted-rotated when the sampling location x is not moved and the signal is simply re-calculated at the location x. In 2D, a signal is virtually shift-rotated when the grid sampling location (x, y) is not moved and the signal is simply re-calculated at (x, y). Similarly, in 3D, a signal is virtually shift-rotated when the 3D grid sampling location (x, y, z) is not moved and the signal is simply re-calculated at (x, y, z). Re-calculation is made through an interpolation formula. An implication of the virtual shift-rotation is that since the grid (node in 1D) is not shifted-rotated, interpolation alone does not suffice to produce any real shift-rotations.


With embedding: In 1D is the act of embedding (including) the signal intensity value located at the center of the neighborhood (see common term section) into the math form of the function, which is usually the interpolation function. The concept is the same in 2D and 3D except that the signal intensity values are located in a 2D neighborhood grid or a 3D neighborhood grid.


Without embedding (WE): In 1D is the act of not embedding (excluding) the signal intensity value located at the center of the neighborhood (see common term section) from the math form of the function, which is usually the interpolation function. The concept is the same in 2D and 3D except that the signal intensity values in a 2D neighborhood grid or a 3D neighborhood grid.


REFERENCES


Ciulla C. & Deek, F. P. (2005). On the approximate nature of the bivariate linear interpolation function: A novel scheme based on intensity-curvature. ICGST - International Journal on Graphics, Vision and Image Processing, 5(7), 9-19.


Carlo Ciulla “Improved Signal and Image Interpolation in Biomedical Applications: The Case of Magnetic Resonance Imaging (MRI)” – Medical Information Science Reference - IGI Global Publisher - March 2009; ISBN: 978 - 160566202 - 2.


Carlo Ciulla “Signal Resilient to Interpolation: An Exploration on the Approximation Properties of the Mathematical Functions” - CreateSpace Publisher - June 2012; pp. 1 - 336, ISBN: 978-1477567487.



#  References


[Add a reference](index.php@title=Odp%253AAdd_reference&subject=Ontology%253ASRE+-+Sub-pixel+Efficacy+Region+&amp%3B+SRI+-+Signal+Resilient+to+Interpolation.html "http://ontologydesignpatterns.org/wiki/index.php?title=Odp:Add_reference&subject=Ontology%3ASRE+-+Sub-pixel+Efficacy+Region+%26amp%3B+SRI+-+Signal+Resilient+to+Interpolation")


  






Retrieved from "[http://ontologydesignpatterns.org/wiki/Ontology:SRE\_-\_Sub-pixel\_Efficacy\_Region\_%26\_SRI\_-\_Signal\_Resilient\_to\_Interpolation](../Ontology/SRE_-_Sub-pixel_Efficacy_Region_&_SRI_-_Signal_Resilient_to_Interpolation)"
 [Category](http://ontologydesignpatterns.org/wiki/Special:Categories "Special:Categories"): [Ontology](../Category/Ontology "Category:Ontology")