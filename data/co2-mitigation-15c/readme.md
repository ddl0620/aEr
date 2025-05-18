# CO₂ reductions needed to keep global temperature rise below 1.5°C - Data package

This data package contains the data that powers the chart ["CO₂ reductions needed to keep global temperature rise below 1.5°C"](https://ourworldindata.org/grapher/co2-mitigation-15c?v=1&csvType=full&useColumnShortNames=false) on the Our World in Data website. It was downloaded on May 16, 2025.

### Active Filters

A filtered subset of the full data was downloaded. The following filters were applied:

## CSV Structure

The high level structure of the CSV file is that each row is an observation for an entity (usually a country or region) and a timepoint (usually a year).

The first two columns in the CSV file are "Entity" and "Code". "Entity" is the name of the entity (e.g. "United States"). "Code" is the OWID internal entity code that we use if the entity is a country or region. For normal countries, this is the same as the [iso alpha-3](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-3) code of the entity (e.g. "USA") - for non-standard countries like historical countries these are custom codes.

The third column is either "Year" or "Day". If the data is annual, this is "Year" and contains only the year as an integer. If the column is "Day", the column contains a date string in the form "YYYY-MM-DD".

The final column is the data column, which is the time series that powers the chart. If the CSV data is downloaded using the "full data" option, then the column corresponds to the time series below. If the CSV data is downloaded using the "only selected data visible in the chart" option then the data column is transformed depending on the chart type and thus the association with the time series might not be as straightforward.

## Metadata.json structure

The .metadata.json file contains metadata about the data package. The "charts" key contains information to recreate the chart, like the title, subtitle etc.. The "columns" key contains information about each of the columns in the csv, like the unit, timespan covered, citation for the data etc..

## About the data

Our World in Data is almost never the original producer of the data - almost all of the data we use has been compiled by others. If you want to re-use data, it is your responsibility to ensure that you adhere to the sources' license and to credit them correctly. Please note that a single time series may have more than one source - e.g. when we stich together data from different time periods by different producers or when we calculate per capita metrics using population data from a second source.

## Detailed information about the data


## CO2 mitigation curves to meet a 1.5C target
The range of CO2 mitigation curves to have a >66% chance of keeping global average temperature rise below 1.5°C. Scenarios measure future global annual emissions necessary based on a given start year for emissions mitigation.
Last updated: December 3, 2019  
Date range: 1750–2100  
Unit: tonnes  


### How to cite this data

#### In-line citation
If you have limited space (e.g. in data visualizations), you can use this abbreviated in-line citation:  
Robbie Andrew – processed by Our World in Data

#### Full citation
Robbie Andrew – processed by Our World in Data. “CO2 mitigation curves to meet a 1.5C target” [dataset]. Robbie Andrew [original data].
Source: Robbie Andrew – processed by Our World In Data

### Additional information about this data
Data denotes the range of CO2 mitigation curves for a range of 'start year scenarios': Scenarios are based on the annual emission reductions necessary to keep global temperature rise below 1.5°C if emissions mitigation was to start in a given year.

For example, 'Start in 2010' marks the necessary future emissions pathway to have a >66% chance of keeping global average temperatures below 1.5°C warming if global CO2 emissions mitigation had started in 2010, very quickly peaking then falling.

Data is sourced from Robbie Andrew, and available for download [here](http://folk.uio.no/roberan/t/global_mitigation_curves.shtml).

Historical emissions to 2017 are sourced from CDIAC/Global Carbon Project, projection to 2018 from Global Carbon Project (Le Quéré et al. 2018).

Global cumulative CO2 emissions budgets are from the IPCC Special Report on 1.5°C (Rogelj et al 2018): 420 GtCO2 for a 66% of 1.5°C and 1170 GtCO2 for a 66% of 2°C. Mitigation curves describe approximately exponential decay pathways such that the quota is never exceeded (see Raupach et al., 2014).


    