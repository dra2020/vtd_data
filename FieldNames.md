## Field Names in CSV files

The CSV field names are constructed as follows:
* For Census CSVs, category_year_set, where 
    * for 2010 shapes, category = 
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
    * for 2020 shapes, category = 
        * Tot = Total
        * Wh = White alone, not Hispanic
        * His = Hispanic
        * BlC = Black alone or in combination with other races, including Hispanic
        * NatC = American Indian and Alaska native alone or in combination with other races, including Hispanic
        * AsnC = Asian alone or in combination with other races, including Hispanic
        * PacC = Native Hawaiian and Pacific Islander alone or in combination with other races, including Hispanic
        * Bl = Black alone, not Hispanic
        * Nat = American Indian and Alaska native alone, not Hispanic
        * Asn = Asian alone, not Hispanic
        * Pac = Native Hawaiian and Pacific Islander alone, not Hispanic
        * OthAl = Other race alone, not Hispanic
        * Mix = Two or more races, not Hispanic
    * set =
        * tot = Total population from Census
        * acstot = Total population from 5-year ACS
        * adjtot = Total (Adjusted) population [with adjusted prisoner population]
        * vap = Voting Age population
        * nhvap = Voting Age population using race alone, not Hispanic data
        * cvap = Citizen Voting Age population from 5-year ACS

* For Election CSVs, party_year_contest[_suffix], where
    * party =
        * Tot = total votes of all parties
        * D = Democratic Party votes
        * R = Republican Party votes
    * contest =
        * pres = President
        * sen = US Senate
        * gov = Governor
        * ltg = Lt. Governor
        * ag = Attorney General
    * suffix =
        * roff = Runoff
        * spec = Special
        * sproff = Special Runoff

