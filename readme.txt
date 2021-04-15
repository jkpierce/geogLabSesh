Here I'm sifting through datasets trying to get ideas. 


----------------------------------------------------------------------------------------------------


I organized all of the BC snowfall data. The key product here is 

"snowWaterEquivalentBC_Apr1.csv" which contains a bunch of stations of snow-water-equivalent sampled on April 1st from 1950 to now. Lots of these show decreasing trends, so it's clear to see that snowfall is decreasing in BC. They especially decrease toward the inland. There is very little change in the lower mainland. 

https://www2.gov.bc.ca/gov/content/environment/air-land-water/water/water-science-data/water-data-tools/snow-survey-data/automated-snow-weather-stations-list

There are "manual" and "automated" datasets which don't download properly in chrome.


----------------------------------------------------------------------------------------------------

Another key product is FraserRiverAnnualExtremes.csv 
This is maximum and minimum annual flows in the fraser from 1912 to 2020.


----------------------------------------------------------------------------------------------------


Another key product here is ens_oni_data_1850-feb_2021.xlsx . This contains ENSO conditions from 1850 to now, at least as they're estimated from some climate models. This will allow us to separate snowfall into El Nino and La Nina conditions, provided these are defined as 5 consecutive months having |ONI|>0.5 per the NOAA definition. http://www.webberweather.com/ensemble-oceanic-nino-index.html # here are 3 month from 1850 


----------------------------------------------------------------------------------------------------

The notebook "collectSnowData.ipynb" is just me fighting in python to collect the data from various sources in a nice format.

----------------------------------------------------------------------------------------------------


Finally "vancouverTemperatureAnomaly.csv" is estimated temperature anomalies in vancouver from 188x to now based on interpolating all available data. The grid size is 5x5 deg^2. That's about 555km on a side. 1 deg = 111km. These data are monthly. So this would be an appropriate characteristic of the salish sea.

https://psl.noaa.gov/data/gridded/tables/temperature.html

original paper here: 

Jones, P.D., Lister, D.H., Osborn, T.J., Harpham, C., Salmon, M. and Morice, C.P., 2012: Hemispheric and large-scale land surface air temperature variations: an extensive revision and an update to 2010. Journal of Geophysical Research, doi:10.1029/2011JD017139.

