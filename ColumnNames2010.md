## Column Names in CSV files

For 2010 VTD Shapes, the CSV field names are constructed as follows:
* For Census CSVs, field_year_dataset, where 
    * field = 
        * Tot = Total
        * Wh = White alone, not Hispanic
        * Bl = Black alone, not Hispanic
        * Hisp = Hispanic
        * Nat = American Indian and Alaska native alone, not Hispanic
        * Asn = Asian alone, not Hispanic
        * Pac = Native Hawaiian and Pacific Islander alone, not Hispanic
        * Oth = Other race and two or more races, not Hispanic
        * Bl+ = Black alone or in combination with other races, including Hispanic
        * Nat+ = American Indian and Alaska native alone or in combination with other races, including Hispanic
        * Asn+ = Asian alone or in combination with other races, including Hispanic
        * Pac+ = Native Hawaiian and Pacific Islander alone or in combination with other races, including Hispanic
    * dataset =
        * tot = Total population from Census
        * acstot = Total population from 5-year ACS
        * adjtot = Total (Adjusted) population [with adjusted prisoner population]
        * vap = Voting Age population
        * nhvap = Voting Age population using race alone, not Hispanic data
        * cvap = Citizen Voting Age population from 5-year ACS

* For Election CSVs, party_year_contest , where
    * party =
        * Tot = total votes of all parties
        * D = Democratic Party votes
        * R = Republican Party votes
    * contest =
        * pres = President

