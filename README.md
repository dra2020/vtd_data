# vtd_data
This repository contains Census and Election Data, aggregated to 2010 and 2020 voting tabulation districts (VTDs), as CSV. Files are organized by geography (e.g. 2010_VTD) and then by state.

## 2010 Shapes
For the states CA, MT, OR and RI we use 2010 Block Groups instead of VTDs. 

The census files contain 2010 demographic data, both total population and voting age population, and 2018 American Community Survey (5-year) population estimates (total population only). All of the data is orginally from the U.S. Census Bureau. The 2018 ACS data was aggregated to 2010 VTDs by Dave's Redistricting.

The election files contain election results from 2008 and 2016-2018. The original data was obtain from various sources, as noted below, and aggregated to 2010 VTDs by Dave's Redistricting.

## 2020 Shapes
For the states CA, HI, OR and WV we use 2020 Block Groups instead of VTDs. Also, for ME, county subdivisions were added for counties with no VTDs.

The census files contain 2010 demographic data, both total population and voting age population, and 2018 and 2019 American Community Survey (5-year) population estimates and citizen voting age population (CVAP) estimates. All of the data is orginally from the U.S. Census Bureau.

The election files will be uploaded for each state after we have 2020 election data for that state.

All data was disaggregated to 2020 census blocks by Dave's Redistricting using the method by Voting and Election Science Team (except 2019 ACS was already done by VEST). (Amos, Brian, 2021, "2020 Census Block Crosswalk Data", https://doi.org/10.7910/DVN/T9VMJO, Harvard Dataverse, V2)

## CVAP Data
The Census provides CVAP estimates with the 5-year ACS data, but those estimates don't have the calculations for the race combinations (e.g. Black Alone or in combination with other races). The 2010 Census data (P.L. 94-171) has those combinations for their Total and VAP data. For our CVAP data we estimate the combinations by adding certain fields (e.g. Black Alone + Black and White + Black and Native American), but we do not use the "Remainder of Two or More Races" field, so our estimates tend to underestimate the combinations, particularly Asian and Pacific.

## Election Data
A number of people and organizations obtained, cleaned and aggeregated election data to produce precinct-level election data we use. The 2016-2018 was presented as shapefiles or geojson files, using the precinct/VTD geography obtained from the individual states for those years. The 2008 data was presented already aggregated to 2010 VTDs.

Election data notes:
* 2008 Presidential data for IN, NC, NM, TX: Stephen Ansolabehere, Jonathan Rodden. 2010 Census Shapefile and Precinct-Level Election Data. Release 2011.
* 2008 Presidential data for AK, AL, AR, AZ, CA, CT, DC, DE, FL, GA, HI, IA, ID, IL, KS, KY, LA, MA, MD, ME, MI, MN, MS, MO, MT, ND, NE, NH, NJ, NV, NY, OH, OK, OR, PA, RI, SC, SD, TN, UT, VA, VT, WA, WI, WV, WY: Steve Gerontakis with assistance by John Mifflin.
* 2008 Presidential data for CO: Tyler Chafee.
* 2014 data for MA, MN, NC, TX: Metric Geometry and Gerrymandering Group (https://mggg.org/).
* 2016 data for OH: Metric Geometry and Gerrymandering Group.
* 2018 data for AR, NV: Open Precincts (Princeton Gerrymandering Project) (https://openprecincts.org/).
* 2018 data for CO, OR: Metric Geometry and Gerrymandering Group (via Princeton Gerrymandering Project).
* 2018 data for WA: MIT Election Data Science Lab (via Princeton Gerrymandering Project).
* All California data, except 2016 with 2010 shapes: California Statewide Database.
* All other election data: Voting and Election Science Team (https://dataverse.harvard.edu/dataverse/electionscience).

## Logs
Two log files are provided for each state. The census log file lists the total population and VAP/CVAP population for each year. The election log file shows the total vote counts for some elections. These can be helpful to compare to other sources to sanity check the data.