# Monthly surface temperature anomalies by decade - Data package

This data package contains the data that powers the chart ["Monthly surface temperature anomalies by decade"](https://ourworldindata.org/grapher/monthly-surface-temperature-anomalies-by-decade?v=1&csvType=full&useColumnShortNames=false) on the Our World in Data website.

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


## 2020s
The difference of a specific month's average surface temperature from the 1991-2020 mean, in degrees Celsius.
Last updated: January 7, 2025  
Date range: 1–12  
Unit: °C  


### How to cite this data

#### In-line citation
If you have limited space (e.g. in data visualizations), you can use this abbreviated in-line citation:  
Contains modified Copernicus Climate Change Service information (2025) – processed by Our World in Data

#### Full citation
Contains modified Copernicus Climate Change Service information (2025) – processed by Our World in Data. “2020s” [dataset]. Contains modified Copernicus Climate Change Service information, “ERA5 monthly averaged data on single levels from 1940 to present 2” [original data].
Source: Contains modified Copernicus Climate Change Service information (2025) – processed by Our World In Data

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


## 2010s
The difference of a specific month's average surface temperature from the 1991-2020 mean, in degrees Celsius.
Last updated: January 7, 2025  
Date range: 1–12  
Unit: °C  


### How to cite this data

#### In-line citation
If you have limited space (e.g. in data visualizations), you can use this abbreviated in-line citation:  
Contains modified Copernicus Climate Change Service information (2025) – processed by Our World in Data

#### Full citation
Contains modified Copernicus Climate Change Service information (2025) – processed by Our World in Data. “2010s” [dataset]. Contains modified Copernicus Climate Change Service information, “ERA5 monthly averaged data on single levels from 1940 to present 2” [original data].
Source: Contains modified Copernicus Climate Change Service information (2025) – processed by Our World In Data

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


## 2000s
The difference of a specific month's average surface temperature from the 1991-2020 mean, in degrees Celsius.
Last updated: January 7, 2025  
Date range: 1–12  
Unit: °C  


### How to cite this data

#### In-line citation
If you have limited space (e.g. in data visualizations), you can use this abbreviated in-line citation:  
Contains modified Copernicus Climate Change Service information (2025) – processed by Our World in Data

#### Full citation
Contains modified Copernicus Climate Change Service information (2025) – processed by Our World in Data. “2000s” [dataset]. Contains modified Copernicus Climate Change Service information, “ERA5 monthly averaged data on single levels from 1940 to present 2” [original data].
Source: Contains modified Copernicus Climate Change Service information (2025) – processed by Our World In Data

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


## 1990s
The difference of a specific month's average surface temperature from the 1991-2020 mean, in degrees Celsius.
Last updated: January 7, 2025  
Date range: 1–12  
Unit: °C  


### How to cite this data

#### In-line citation
If you have limited space (e.g. in data visualizations), you can use this abbreviated in-line citation:  
Contains modified Copernicus Climate Change Service information (2025) – processed by Our World in Data

#### Full citation
Contains modified Copernicus Climate Change Service information (2025) – processed by Our World in Data. “1990s” [dataset]. Contains modified Copernicus Climate Change Service information, “ERA5 monthly averaged data on single levels from 1940 to present 2” [original data].
Source: Contains modified Copernicus Climate Change Service information (2025) – processed by Our World In Data

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


## 1980s
The difference of a specific month's average surface temperature from the 1991-2020 mean, in degrees Celsius.
Last updated: January 7, 2025  
Date range: 1–12  
Unit: °C  


### How to cite this data

#### In-line citation
If you have limited space (e.g. in data visualizations), you can use this abbreviated in-line citation:  
Contains modified Copernicus Climate Change Service information (2025) – processed by Our World in Data

#### Full citation
Contains modified Copernicus Climate Change Service information (2025) – processed by Our World in Data. “1980s” [dataset]. Contains modified Copernicus Climate Change Service information, “ERA5 monthly averaged data on single levels from 1940 to present 2” [original data].
Source: Contains modified Copernicus Climate Change Service information (2025) – processed by Our World In Data

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


## 1970s
The difference of a specific month's average surface temperature from the 1991-2020 mean, in degrees Celsius.
Last updated: January 7, 2025  
Date range: 1–12  
Unit: °C  


### How to cite this data

#### In-line citation
If you have limited space (e.g. in data visualizations), you can use this abbreviated in-line citation:  
Contains modified Copernicus Climate Change Service information (2025) – processed by Our World in Data

#### Full citation
Contains modified Copernicus Climate Change Service information (2025) – processed by Our World in Data. “1970s” [dataset]. Contains modified Copernicus Climate Change Service information, “ERA5 monthly averaged data on single levels from 1940 to present 2” [original data].
Source: Contains modified Copernicus Climate Change Service information (2025) – processed by Our World In Data

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


## 1960s
The difference of a specific month's average surface temperature from the 1991-2020 mean, in degrees Celsius.
Last updated: January 7, 2025  
Date range: 1–12  
Unit: °C  


### How to cite this data

#### In-line citation
If you have limited space (e.g. in data visualizations), you can use this abbreviated in-line citation:  
Contains modified Copernicus Climate Change Service information (2025) – processed by Our World in Data

#### Full citation
Contains modified Copernicus Climate Change Service information (2025) – processed by Our World in Data. “1960s” [dataset]. Contains modified Copernicus Climate Change Service information, “ERA5 monthly averaged data on single levels from 1940 to present 2” [original data].
Source: Contains modified Copernicus Climate Change Service information (2025) – processed by Our World In Data

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


## 1950s
The difference of a specific month's average surface temperature from the 1991-2020 mean, in degrees Celsius.
Last updated: January 7, 2025  
Date range: 1–12  
Unit: °C  


### How to cite this data

#### In-line citation
If you have limited space (e.g. in data visualizations), you can use this abbreviated in-line citation:  
Contains modified Copernicus Climate Change Service information (2025) – processed by Our World in Data

#### Full citation
Contains modified Copernicus Climate Change Service information (2025) – processed by Our World in Data. “1950s” [dataset]. Contains modified Copernicus Climate Change Service information, “ERA5 monthly averaged data on single levels from 1940 to present 2” [original data].
Source: Contains modified Copernicus Climate Change Service information (2025) – processed by Our World In Data

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


## 1940s
The difference of a specific month's average surface temperature from the 1991-2020 mean, in degrees Celsius.
Last updated: January 7, 2025  
Date range: 1–12  
Unit: °C  


### How to cite this data

#### In-line citation
If you have limited space (e.g. in data visualizations), you can use this abbreviated in-line citation:  
Contains modified Copernicus Climate Change Service information (2025) – processed by Our World in Data

#### Full citation
Contains modified Copernicus Climate Change Service information (2025) – processed by Our World in Data. “1940s” [dataset]. Contains modified Copernicus Climate Change Service information, “ERA5 monthly averaged data on single levels from 1940 to present 2” [original data].
Source: Contains modified Copernicus Climate Change Service information (2025) – processed by Our World In Data

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


    