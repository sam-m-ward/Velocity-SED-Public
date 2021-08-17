# Velocity-SED-Public
Velocity Correlations with SN Ia SEDs-Public
Project for the Cambridge Spark Accelerate Data Science Residency Program 19/07/21-20/08/21

This notebook uses the BayeSN M20 and T21 models (Mandel et al. 2020, Thorp et al. 2021) of Type Ia Supernova Spectral Energy Distributions, 
along with velocity measurements of the Silicon II line from Dettman et al. 2021,
to search for correlations between velocity and light curve features in various passbands/phases.

We use 
Foundation survey data [griz passbands] (Foley et al. (2018); Jones et al. (2019))) 
fitted using BayeSN T21
and 
CSP survey data [BVRIYJH passbands] (Hamuy et al. (2006); Contreras et al. (2010); Wang et al. (2009); Foley & Kasen (2011); Folatelli et al. (2010);
Stritzinger et al. (2011); Krisciunas et al. (2017)) 
fitted using BayeSN M20.

The notebook loops through features, and performs a KS test on feature sub-samples split at the median velocity. 

The end products are p-value pandas data frames, and heatmaps of the pvalues with time on the x and y axes.

For the purposes of this public notebook release, the data has been limited to [gr] for Foundation, and [BV] for CSP.

Author: S. M. Ward; Acknowledgements: M. Boresta, K. Mandel, S. Thorp
