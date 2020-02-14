# vtd_data
This repository contains Census and Election Data, aggregated to 2010 voting tabulation district (VTD) geometry, as CSV. (Note: for the following states we use 2010 Block Group geometry instead of VTD: CA, MT, OR, RI.) Files are organized by geometry (2010_VTD) and then by state.

The census files contain 2010 demographic data, both total population and voting age population, and 2018 American Community Survey (5-year) population estimates (total population only). All of the data is orginally from the U.S. Census Bureau. The 2018 ACS data was aggregated to 2010 VTDs by Dave's Redistricting.

The election files contain election results from 2008 and 2016-2018. The original data was obtain from various sources, as noted below, and aggregated to 2010 VTDs by Dave's Redistricting.

## Election Data
A number of people and organizations obtained, cleaned and aggeregated election data to produce the source data for our election data. The 2016-2018 was presented to us as shapefiles or .geojson files, using the voting district/precinct geometry obtained from the individual states for those years. Dave's Redistricting aggregated that data to the 2010 VTD geometry. The 2008 data was presented to us already aggregated to the 2010 VTD geometry.

Election data notes:
* 2008 Presidential election data for IN, NC, NM, TX: Stephen Ansolabehere, Jonathan Rodden. 2010 Census Shapefile and Precinct-Level Election Data. Release 2011.
* 2008 Presidential election data for AK, AL, AR, AZ, CA, CT, DC, DE, FL, GA, HI, IA, ID, IL, KS, KY, LA, MA, MD, ME, MI, MN, MS, MO, MT, ND, NE, NH, NJ, NV, NY, OH, OK, OR, PA, RI, SC, SD, TN, UT, VA, VT, WA, WI, WV, WY: Steve Gerontakis with assistance by John Mifflin.
* 2008 Presidential data for CO: Tyler Chafee.
* 2012 Presidential data for KS: Voting and Election Science Team, 2019, "2012 Precinct-Level Election Results", Harvard Dataverse.
* 2016 Presidential data, plus 2016 election data for other contests for AK, AR, AZ, CA, CO, DE, FL, GA, HI, IA, IL, KS, MA, MD, ME, MI, MN, MO, MT, NC, ND, NE, NH, NM, NV, OK, OR, RI, SC, TN, TX, UT, VA, VT, WA, WI, WY: Voting and Election Science Team, 2018, "2016 Precinct-Level Election Results", Harvard Dataverse.
* 2017/2018 election data for AZ, IA, ME, MT, ND, OK, RI, VA, VT, WI: Voting and Election Science Team, 2019, "2018 Precinct-Level Election Results", Harvard Dataverse.
* 2018 election data for NV: Open Precincts (Princeton Gerrymandering Project).

## Logs
Two log files are provided for each state. The census log file lists the percentage of population decline in any VTDs where population decreased between 2010 and 2018, along with total population for 2010 and 2018. (Note the 2018 population is the 5-year estimate and tends to be below the 1-year 2018 estimate.)

The election log file shows the total vote counts for 2008 President and, if available, 2016 President and 2018 Senate. These can be helpful to compare to other sources to sanity check the disaggregation/aggregation process. See Disaggregation.md for notes on that process.