# How-much-did-it-rain
Predicting rainfall given the polarimetric radar measurements 

For agriculture, it is extremely important to know how much it rained on a particular field. However, rainfall is variable in space and time and it is impossible to have rain gauges everywhere. 
Therefore, remote sensing instruments such as radar are used to provide wide spatial coverage.

Rainfall estimates drawn from remotely sensed observations will never exactly match the measurements that are carried out using rain gauges, due to the inherent characteristics of both sensors. Currently, radar observations are "corrected" using nearby gauges and a single estimate of rainfall is provided to users who need to know how much it rained.


## POLARIMETRIC RADAR MEASUREMENTS

Unlike a conventional Doppler radar, a polarimetric radar transmits radio wave pulses that have both horizontal and vertical orientations. Because rain drops become flatter as they increase in size and because ice crystals tend to be elongated vertically, whereas liquid droplets tend to be flattened, it is possible to infer the size of rain drops and the type of hydrometeor from the differential reflectivity of the two orientations.
The US National Weather Service's weather radar network (called NEXRAD) was recently upgraded to polarimetry.

The Challenge is to solve this in probabilistic manner.Knowing the full probabilistic spread of rainfall amounts can be very useful to drive hydrological and agronomic models -- much more than a single estimate of rainfall.
We are given polarimetric radar values and derived quantities at a location over the period of one hour. You will need to produce a probabilistic distribution of the hourly rain gauge total. 



## DATA
The training data consists of NEXRAD and MADIS data collected the first 8 days of Apr to Nov 2013 over midwestern corn-growing states. Time and location information have been censored, and the data have been shuffled so that they are not ordered by time or place. 
The test data consists of data from the same radars and gauges over the same months but in 2014

### About the files:

PredictingRainfall.iypnb contains the code and how_much_did_it_rain.pdf contains the documentation of my approach.

With this method I got a rank of 31 in private leaderboard. 

The link for the competition is https://www.kaggle.com/c/how-much-did-it-rain. 

The train and test data can be downloaded here:
https://www.kaggle.com/c/how-much-did-it-rain/data
