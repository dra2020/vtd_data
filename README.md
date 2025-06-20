# vtd_data
This repository contains Demographic and Election Data, aggregated to 2010 and 2020 voting tabulation districts (VTDs), as CSV files and (2020 VTDs only) GeoJSON files. The files are organized by geography (e.g. 2020_VTD) and then by state.

YOU ARE RESPONSIBLE FOR READING AND UNDERSTANDING THE LICENSES FOR THIS DATA, INCLUDING INDIVIDUAL DATASET LICENSES IF ANY.

YOU AGREE NOT TO SELL ANY OF THIS DATA UNDER ANY CIRCUMSTANCES.

## 2010 Shapes
For 2010 Shapes, two CSVs are available for download: one with demographic data and one with election data.

For the states CA, MT, OR and RI we use 2010 Block Groups instead of VTDs. 

The census files contain 2010 demographic data from the decennial census, both total population and voting age population, and 2018 American Community Survey (5-year) population estimates (total population only). All of the data is orginally from the U.S. Census Bureau. The 2018 ACS data was aggregated to 2010 VTDs by Dave's Redistricting.

The election files contain presidential election results from 2008. The original data was obtain from sources noted below and aggregated to 2010 VTDs by Dave's Redistricting.
* 2008 Presidential data for IN, NC, NM, TX: Stephen Ansolabehere, Jonathan Rodden. 2010 Census Shapefile and Precinct-Level Election Data. Release 2011.
* 2008 Presidential data for AK, AL, AR, AZ, CA, CT, DC, DE, FL, GA, HI, IA, ID, IL, KS, KY, LA, MA, MD, ME, MI, MN, MS, MO, MT, ND, NE, NH, NJ, NV, NY, OH, OK, OR, PA, RI, SC, SD, TN, UT, VA, VT, WA, WI, WV, WY: Steve Gerontakis with assistance by John Mifflin.
* 2008 Presidential data for CO: Tyler Chafee.

## 2020 Shapes
For 2020 Shapes, three zip archives are available for download: one with demographic data (CSV), one with election data (CSV), and a GeoJSON with VTD shapes and all demographic and election data. The CSV archives contains a CSV with the data, a license file and a readme with other details. For all states except FL and ME, a link to the VTD or Block Group shapes (on the Census Bureau's site) is provided. For FL and ME a geojson file with the shapes is provided. The GeoJSON archive contains the GeoJSON file, a license file, a readme, and a VTD adjacency file.

For the states CA, HI, OR and WV we use 2020 Block Groups instead of VTDs. For ME, county subdivisions were added for counties with no VTDs. FL uses VTDs, but we made several corrections in two counties.

The census files contain 2010 and 2020 demographic data from the decennial census, both total population and voting age population, and 2018, 2019, 2020 and 2022 American Community Survey (5-year) population estimates and citizen voting age population (CVAP) estimates. All of the data is orginally from the U.S. Census Bureau.

We have election data through 2021 for each state and 2022 and 2024 data for some states.
* Most election data was obtained from Voting and Election Science Team (https://dataverse.harvard.edu/dataverse/electionscience). This data is available under the Creative Commons Attribution license (CC BY 4.0, https://creativecommons.org/licenses/by/4.0/).
* Please see About Data (https://davesredistricting.org/maps#aboutdata) for complete information on data sources. Also, each download specifies the data source and license information.

All data was disaggregated to 2020 census blocks by Dave's Redistricting using the method by Voting and Election Science Team (Amos, Brian, 2021, "2020 Census Block Crosswalk Data", https://doi.org/10.7910/DVN/T9VMJO, Harvard Dataverse, V2), except 2019 ACS data was disaggregated by VEST and 2020 CVAP data was disaggregated by Redistricting Data Hub (https://redistrictingdatahub.org/data/about-our-data/american-community-survey/#cvap).

## CVAP Data
The Census Bureau provides CVAP estimates with the 5-year ACS data, but those estimates don't have the calculations for the race combinations (e.g. "Black Alone or in combination with other races"). The CVAP data only includes these two-race combinations: "Native and White", "Asian and White", "Black and White", "Native and Black", plus "Remainder of Two or More Races". We estimate the combinations by adding those two-race combinations, but leaving out the remainder, which tends to underestimate the race combinations.

## Logs
Two log files are provided for each state from the production of the CSVs, which list two totals for all of the fields, one from the block data and one from the data aggregated to the VTDs, plus a difference (which should be 0). A third log file is provided for each state from the production of the GeoJSON.
