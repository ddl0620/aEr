# Ice sheet mass balance - Data package

This data package contains the data that powers the chart ["Ice sheet mass balance"](https://ourworldindata.org/grapher/ice-sheet-mass-balance?v=1&csvType=full&useColumnShortNames=false) on the Our World in Data website. It was downloaded on May 14, 2025.

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


## Cumulative change in mass in the ice sheets, according to NASA/JPL – NASA/JPL
Measured in billion tonnes.
Last updated: March 17, 2025  
Next update: May 2025  
Unit: billion tonnes  


### How to cite this data

#### In-line citation
If you have limited space (e.g. in data visualizations), you can use this abbreviated in-line citation:  
EPA based on various sources (2021) – with major processing by Our World in Data

#### Full citation
EPA based on various sources (2021) – with major processing by Our World in Data. “Cumulative change in mass in the ice sheets, according to NASA/JPL – NASA/JPL” [dataset]. United States Environmental Protection Agency, “Climate Change Indicators: Ice Sheets” [original data].
Source: EPA based on various sources (2021) – with major processing by Our World In Data

### What you should know about this data
* Values are centered at zero in 2002 to provide a consistent point of reference.
* A downward slope indicates a net loss of ice and snow.
* For reference, 1,000 billion metric tons is enough to raise sea level by about 3 millimeters.

### Source

#### United States Environmental Protection Agency – Climate Change Indicators: Ice Sheets
Retrieved on: 2024-04-17  
Retrieved from: https://www.epa.gov/climate-indicators/climate-change-indicators-ice-sheets  


    