# Deaths in armed conflicts by region - Data package

This data package contains the data that powers the chart ["Deaths in armed conflicts by region"](https://ourworldindata.org/grapher/deaths-in-armed-conflicts-by-region?v=1&csvType=full&useColumnShortNames=false) on the Our World in Data website. It was downloaded on June 3, 2026.

### Active Filters

A filtered subset of the full data was downloaded. The following filters were applied:

## CSV Structure

The high level structure of the CSV file is that each row is an observation for an entity (usually a country or region) and a timepoint (usually a year).

The first two columns in the CSV file are "Entity" and "Code". "Entity" is the name of the entity (e.g. "United States"). "Code" is the OWID internal entity code that we use if the entity is a country or region. For most countries, this is the same as the [iso alpha-3](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-3) code of the entity (e.g. "USA") - for non-standard countries like historical countries these are custom codes.

The third column is either "Year" or "Day". If the data is annual, this is "Year" and contains only the year as an integer. If the column is "Day", the column contains a date string in the form "YYYY-MM-DD".

The final column is the data column, which is the time series that powers the chart. If the CSV data is downloaded using the "full data" option, then the column corresponds to the time series below. If the CSV data is downloaded using the "only selected data visible in the chart" option then the data column is transformed depending on the chart type and thus the association with the time series might not be as straightforward.


## Metadata.json structure

The .metadata.json file contains metadata about the data package. The "charts" key contains information to recreate the chart, like the title, subtitle etc.. The "columns" key contains information about each of the columns in the csv, like the unit, timespan covered, citation for the data etc..

## About the data

Our World in Data is almost never the original producer of the data - almost all of the data we use has been compiled by others. If you want to re-use data, it is your responsibility to ensure that you adhere to the sources' license and to credit them correctly. Please note that a single time series may have more than one source - e.g. when we stich together data from different time periods by different producers or when we calculate per capita metrics using population data from a second source.

## Detailed information about the data


## Deaths in armed conflicts
The best estimate of the number of deaths of combatants and civilians due to fighting in interstate, intrastate, extrasystemic, non-state conflicts, and one-sided violence that were ongoing that year.
Last updated: May 1, 2026  
Date range: 1989–2026  
Unit: deaths  


### How to cite this data

#### In-line citation
If you have limited space (e.g. in data visualizations), you can use this abbreviated in-line citation:  
Uppsala Conflict Data Program (2025); Uppsala Conflict Data Program (2026); geoBoundaries (2023) – processed by Our World in Data

#### Full citation
Uppsala Conflict Data Program (2025); Uppsala Conflict Data Program (2026); geoBoundaries (2023) – processed by Our World in Data. “Deaths in armed conflicts” [dataset]. Uppsala Conflict Data Program, “Georeferenced Event Dataset v25.1”; Uppsala Conflict Data Program, “Candidate Events Dataset v25.01.25.12”; Uppsala Conflict Data Program, “Candidate Events Dataset v26.01.26.03”; geoBoundaries, “geoBoundaries - Comprehensive Global Administrative Zones (CGAZ) 6.0.0” [original data].
Source: Uppsala Conflict Data Program (2025), Uppsala Conflict Data Program (2026), geoBoundaries (2023) – processed by Our World In Data

### What you should know about this data
* An armed conflict is defined by the [Uppsala Conflict Data Program (UCDP)](https://ucdp.uu.se/) as a disagreement between organized groups, or between one organized group and civilians, that causes at least 25 deaths during a year. This includes combatant and civilian deaths due to fighting.
* This includes [interstate conflicts](#dod:interstate-ucdp), [civil conflicts](#dod:intrastate-ucdp), [non-state conflicts](#dod:nonstate-ucdp), [violence against civilians](#dod:onesided-ucdp), and [colonial conflicts](#dod:extrasystemic-ucdp).
* UCDP identifies conflict deaths [based on news reports, other contemporary sources, and academic research](https://www.uu.se/en/department/peace-and-conflict-research/research/ucdp/ucdp-methodology).
* UCDP's data for 2025 and 2026 is preliminary. This means the number of deaths may be too low because more information becomes available later, or they may be too high because some events are later found not to be part of an armed conflict. In addition, data for 2026 only covers the first quarter of the year. We still show this data to provide more up-to-date information, but figures on this chart may change in the future if UCDP revises its estimates.
* We use UCDP's quarterly [Candidate Events Datasets](https://ucdp.uu.se/downloads/) for the preliminary data. We add data for the first quarter of the current year in May, for the second quarter in August, for the third quarter in November, and for the fourth quarter in February.
* We show here the "best" death estimates as identified by UCDP. They also report high and low estimates.

### Sources

#### Uppsala Conflict Data Program – Georeferenced Event Dataset
Retrieved on: 2025-06-13  
Retrieved from: https://ucdp.uu.se/downloads/index.html#ged_global  

#### Uppsala Conflict Data Program – Candidate Events Dataset
Retrieved on: 2026-02-16  
Retrieved from: https://ucdp.uu.se/downloads/index.html#candidate  

#### geoBoundaries – geoBoundaries - Comprehensive Global Administrative Zones (CGAZ)
Retrieved on: 2025-06-26  
Retrieved from: https://www.geoboundaries.org/globalDownloads.html  

#### Notes on our processing step for this indicator
UCDP provides geographical coordinates of each conflict event. We have mapped these coordinates to countries by means of the geoBoundaries dataset.

In some instances, the event's coordinates fall within the borders of a country. Other times, the event's coordinates fall outside the borders of a country. In the latter case, we have mapped the event to the country that is closest to the event's coordinates.

Conflict event with id "53238" and relid "PAK-2003-1-345-88" was assigned to "Siachen-Saltoro" by geoBoundaries. We have mapped it to "Pakistan" following the text in the `where_description` field from the UCDP data, which refers to "Giang sector in Siachen, Pakistani Kashmir".


    