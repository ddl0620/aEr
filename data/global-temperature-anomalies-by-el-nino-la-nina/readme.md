# Global temperature anomalies by El Niño and La Niña conditions - Data package

This data package contains the data that powers the chart ["Global temperature anomalies by El Niño and La Niña conditions"](https://ourworldindata.org/grapher/global-temperature-anomalies-by-el-nino-la-nina?v=1&csvType=full&useColumnShortNames=false) on the Our World in Data website.

## CSV Structure

The high level structure of the CSV file is that each row is an observation for an entity (usually a country or region) and a timepoint (usually a year).

The first two columns in the CSV file are "Entity" and "Code". "Entity" is the name of the entity (e.g. "United States"). "Code" is the OWID internal entity code that we use if the entity is a country or region. For normal countries, this is the same as the [iso alpha-3](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-3) code of the entity (e.g. "USA") - for non-standard countries like historical countries these are custom codes.

The third column is either "Year" or "Day". If the data is annual, this is "Year" and contains only the year as an integer. If the column is "Day", the column contains a date string in the form "YYYY-MM-DD".

The remaining columns are the data columns, each of which is a time series. If the CSV data is downloaded using the "full data" option, then each column corresponds to one time series below. If the CSV data is downloaded using the "only selected data visible in the chart" option then the data columns are transformed depending on the chart type and thus the association with the time series might not be as straightforward.

## Metadata.json structure

The .metadata.json file contains metadata about the data package. The "charts" key contains information to recreate the chart, like the title, subtitle etc.. The "columns" key contains information about each of the columns in the csv, like the unit, timespan covered, citation for the data etc..

## About the data

Our World in Data is almost never the original producer of the data - almost all of the data we use has been compiled by others. If you want to re-use data, it is your responsibility to ensure that you adhere to the sources' license and to credit them correctly. Please note that a single time series may have more than one source - e.g. when we stich together data from different time periods by different producers or when we calculate per capita metrics using population data from a second source.

### How we process data at Our World In Data
All data and visualizations on Our World in Data rely on data sourced from one or several original data providers. Preparing this original data involves several processing steps. Depending on the data, this can include standardizing country names and world region definitions, converting units, calculating derived indicators such as per capita measures, as well as adding or adapting metadata such as the name or the description given to an indicator.
[Read about our data pipeline](https://docs.owid.io/projects/etl/)

## Detailed information about each time series


## Temperature anomaly
The difference of a specific month's average surface temperature from the 1991-2020 mean, in degrees Celsius.
Last updated: January 7, 2025  
Unit: °C  


### How to cite this data

#### In-line citation
If you have limited space (e.g. in data visualizations), you can use this abbreviated in-line citation:  
Contains modified Copernicus Climate Change Service information (2025) – with major processing by Our World in Data

#### Full citation
Contains modified Copernicus Climate Change Service information (2025) – with major processing by Our World in Data. “Temperature anomaly” [dataset]. Contains modified Copernicus Climate Change Service information, “ERA5 monthly averaged data on single levels from 1940 to present 2” [original data].
Source: Contains modified Copernicus Climate Change Service information (2025) – with major processing by Our World In Data

### Source

#### Contains modified Copernicus Climate Change Service information – ERA5 monthly averaged data on single levels from 1940 to present
Retrieved on: 2025-04-07  
Retrieved from: https://cds.climate.copernicus.eu/datasets/reanalysis-era5-single-levels-monthly-means?tab=overview  

#### Notes on our processing step for this indicator
- Temperature measured in kelvin was converted to degrees Celsius (°C) by subtracting 273.15.

- Initially, the temperature dataset is provided with specific coordinates in terms of longitude and latitude. To tailor this data to each country, we utilize geographical boundaries as defined by the World Bank. The method involves trimming the global temperature dataset to match the exact geographical shape of each country. To correct for potential distortions caused by the Earth's curvature on a flat map, we apply a latitude-based weighting. This step is essential for maintaining accuracy, especially in high-latitude regions where distortion is more pronounced. The result of this process is a latitude-weighted average temperature for each nation.

- It's important to note, however, that due to the resolution constraints of the Copernicus dataset, this methodology might not be as effective for countries with very small landmasses. In these cases, the process may not yield reliable data.

- The derived 2-meter temperature readings for each country are calculated based on administrative borders, encompassing all land surface types within these defined areas. As a result, temperatures over oceans and seas are not included in these averages, focusing the data primarily on terrestrial environments.

- Global temperature averages and anomalies are calculated over all land and ocean surfaces.
- The temperature anomaly is calculated by comparing the average surface temperature of a specific time period (e.g., a particular year or month) to the mean surface temperature of the same period from 1991 to 2020.

- When calculating anomalies for each country, the average surface temperature of a given year or month is compared to the 1991-2020 mean temperature for that specific country.

- The reason for using the 1991-2020 period as the reference mean is that it is the standard reference period used by our data source, the Copernicus Climate Change Service. This period is also adopted by the UK Met Office. This approach ensures consistency in identifying climate variations over time.


## Oceanic Niño Index (ONI) anomaly
The Oceanic Niño Index (ONI) anomaly is a measure of the sea surface temperature anomalies in the east-central tropical Pacific Ocean.
Last updated: February 12, 2025  
Next update: June 2025  


### How to cite this data

#### In-line citation
If you have limited space (e.g. in data visualizations), you can use this abbreviated in-line citation:  
NOAA National Centers for Environmental Information (2025) – with minor processing by Our World in Data

#### Full citation
NOAA National Centers for Environmental Information (2025) – with minor processing by Our World in Data. “Oceanic Niño Index (ONI) anomaly” [dataset]. NOAA National Centers for Environmental Information, “Equatorial Pacific Sea Surface Temperatures (SST) data” [original data].
Source: NOAA National Centers for Environmental Information (2025) – with minor processing by Our World In Data

### What you should know about this data
* The Oceanic Niño Index (ONI) is a tool used by the National Oceanic and Atmospheric Administration (NOAA) to monitor and track the presence and intensity of El Niño and La Niña events.
* These events are part of the broader El Niño-Southern Oscillation (ENSO), a natural climate pattern that affects global weather patterns, including rainfall, droughts, and hurricane activity.
* The ONI measures deviations in sea surface temperatures (SSTs) in a specific area of the Pacific Ocean, known as the Niño 3.4 region. This region spans from 120°W to 170°W longitude, along the equator, in the east-central tropical Pacific.
* NOAA calculates the ONI by taking a 3-month running mean of SST anomalies. An anomaly is the difference between observed SSTs and the 30-year climatological average for the same period. NOAA periodically updates the baseline period to ensure consistency with long-term climate trends. For example, the 1991–2020 average is often used.
* El Niño (ONI ≥ +0.5°C) occurs when sea surface temperatures in the Niño 3.4 region are warmer than usual, often bringing drier conditions to Asia and Australia, wetter weather to the southern United States, and weakened trade winds.
* El Niño can lead to weaker Atlantic hurricane seasons but stronger and more frequent Pacific hurricanes.
* Neutral (−0.5°C < ONI < +0.5°C) means sea surface temperatures are near average, with no significant ENSO event.
* La Niña (ONI ≤ −0.5°C) happens when sea surface temperatures are cooler than usual, often causing drier conditions in South America, increased rainfall in Indonesia and northern Australia, and stronger trade winds.
* La Niña tends to cause more hurricanes in the Atlantic and drought conditions in the southern U.S.

### How is this data described by its producer - NOAA National Centers for Environmental Information (2025)?
- El Niño (La Niña) is a phenomenon in the equatorial Pacific Ocean characterized by a five consecutive 3-month running mean of sea surface temperature (SST) anomalies in the Niño 3.4 region that is above (below) the threshold of +0.5°C (-0.5°C). This standard of measure is known as the Oceanic Niño Index (ONI).
- Historically, scientists have classified the intensity of El Niño based on SST anomalies exceeding a pre-selected threshold in a certain region of the equatorial Pacific. The most commonly used region is the Niño 3.4 region, and the most commonly used threshold is a positive SST departure from normal greater than or equal to +0.5°C. Since this region encompasses the western half of the equatorial cold tongue region, it provides a good measure of important changes in SST and SST gradients that result in changes in the pattern of deep tropical convection and atmospheric circulation. The criteria, that is often used to classify El Niño episodes, is that five consecutive 3-month running mean SST anomalies exceed the threshold.
- Studies have shown that a necessary condition for the development and persistence of deep convection (enhanced cloudiness and precipitation) in the Tropics is that the local SST be 28°C or greater. Once the pattern of deep convection has been altered due to anomalous SSTs, the tropical and subtropical atmospheric circulation adjusts to the new pattern of tropical heating, resulting in anomalous patterns of precipitation and temperature that extend well beyond the region of the equatorial Pacific. An SST anomaly of +0.5°C in the Niño 3.4 region is sufficient to reach this threshold from late March to mid-June. During the remainder of the year a larger SST anomaly, up to +1.5°C in November-December-January, is required in order to reach the threshold to support persistent deep convection in that region.
- SST values in the Niño 3.4 region may not be the best choice for determining La Niña episodes but, for consistency, the index has been defined by negative anomalies in this area. A better choice might be the Niño 4 region, since that region normally has SSTs at or above the threshold for deep convection throughout the year. An SST anomaly of -0.5°C in that region would be sufficient to bring water temperatures below the 28°C threshold, which would result in a significant westward shift in the pattern of deep convection in the tropical Pacific.

### Source

#### NOAA National Centers for Environmental Information – Equatorial Pacific Sea Surface Temperatures (SST) data
Retrieved on: 2025-04-07  
Retrieved from: https://www.ncei.noaa.gov/access/monitoring/enso/sst  


    