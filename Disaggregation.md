## Disaggregation and Aggregation

To map election results and demographic data from a source geometry (shape set) to a destination geometry (shape set), we disaggregate the data from the source geometry to census blocks and then aggregate from those to the destination geometry.

For example, 2016 election data for many states is presented in terms of each state's 2016 precincts (or voting districts), which typically differ from their 2010 precincts. The representation of those precincts on a map is the geometry with which that election data is associated. Our algorithm determines the geometric mapping between the 2016 precincts and 2010 census blocks and then distributes the results for each precinct among the blocks in that precinct, according to the 2010 voting age population of each block. (That's disaggregation.) The Census Bureau provides the mapping between census blocks and the 2010 precincts and using that we add the results from all the blocks in each precinct. (That's aggregation.)

We compared the aggregated data to the original to see how many votes were "lost" in the process. For most states less than 0.01% of votes were lost for most contests. But a few had larger losses, which are noted below.
* CA: up to 0.15% lost
* FL: up to 0.3% lost
* WI: up to 0.2% lost