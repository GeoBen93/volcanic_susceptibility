# volcanic_susceptibility
Model for prediciting the location of future volcanic vents based on the location of pervious eruptions. The code is provided as a jupyter notebook and was developed in the thesis of Ben Clarke 2019 (University of Edinburgh) entitled 'Post-caldera eruptions and pyroclastic density current hazards in the Main Ethiopian Rift'. 

The model requires two inputs, a list of volcanic vent locations (UTMx and UTMy coordinates), and a list of coordinates where you wish to estimate the vent opening probabilities. Examples are provided for Aluto volcano in Ethiopia. 

The model employs the approach described in Weller et al. 2006., where it is used to estimate the location of future monogentetic volcanism around a geothermal power station in Armenia. For a detailed exaplanation of the mathematics and model assumptions, please refer to this source material. 

The approach is a kernel density estimation. Where the bandwidth of a Gaussian kernel is assigned based upon the nearest neighbour distances of existing volcanic vents. The underlying assumption is that volcanic vent opening in this system is a non-homogeneous poisson point process. 
