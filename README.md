# General sensitivity of Indonesia’s rainfall: pixel-wise regression between rainfall and sea surface temperature

Climate variability directly influences many aspects of food and nutrition security, particularly food availability and access. Variation in rainfall is a common element of many natural disasters – droughts, floods, typhoons and tsunamis – and is influenced by global, regional and/or local factors. 

Global climate factors including El Niño, La Niña and the dipole mode; regional factors include monsoon circulation, the Madden-Julian oscillation and fluctuations in the surface temperature of the Indonesian Sea; and local factors can include elevation, island position, the circulation of land and sea breezes, and land cover.

The level of climate risk is measured based on the strength of ENSO signal on rainfall variability using correlation analysis. This approach is applied because production loss of food crops in Indonesia is closely associated with the ENSO phenomena. El Nino years is normally associated with drought years, while La-Nina is often related to wet years which can cause flood hazards. The correlation analysis is applied to monthly rainfall anomaly and sea surface temperature anomaly in NINO3.4.

The NINO-3.4 region is optimal for monitoring El Niño-Southern Oscillation (ENSO) and its impacts in Indonesia and possibly Southeast Asia.
 
## Objective
Change in rainfall with 1° increase in sea surface temperature (SST) of NINO-3.4 region, as a signal for moderate El Niño.

## Method
- **Calculate monthly rainfall anomaly** The anomaly is calculated as the following:
Anomaly(X)ii = Xij – mean(X)i
Where Xij is data of month-i in year-j while mean(X)i is average data for month-i over a number of years.
- **Simple regression** will apply to indicate the correlation between rainfall anomaly in each area to anomaly of SST in the Pacific Ocean which represent ENSO signals. Y = a + bX, where: Y = Rainfall anomaly, a = Y intercept, b = Slope, X = SST anomaly, If the correlation is not significant (p-value > 0.05, slope is set to 0 (zero).

## Data
- 35 years (1981-2017) monthly rainfall data used in the analysis are downloaded from Climate Hazards Center - UC Santa Barbara (https://chc.ucsb.edu/data-sets/chirps), and 
- SST anomaly in NINO-3.4 region from ERSST v5 of National Oceanic and Atmospheric Administration (NOAA) (https://www.cpc.ncep.noaa.gov/products/analysis_monitoring/ensostuff/detrend.nino34.ascii.txt). 

## Output
- A raster file (GeoTIFF) from the slope and correlation of both data.
- R script for the pixel-wise regression.
- Documentation on the approach and work steps.

## References
- https://matinbrandt.wordpress.com/2014/05/26/pixel-wise-regression-between-two-raster-time-series/ 
- https://www.hakimabdi.com/blog/test-pixelwise-correlation-between-two-time-series-of-raster-data-in-r?format=amp 
