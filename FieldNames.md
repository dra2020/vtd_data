## Field Names in CSV files

The CSV field names are constructed as follows:
* For Census CSVs, <category>_<year>_<set>, where 
    * category = 
        * Tot = Total
        * Wh = White alone, not Hispanic
        * Bl = Black alone, not Hispanic
        * Hisp = Hispanic
        * Nat = American Indian and Alaska native alone, not Hispanic
        * Asn = Asian alone, not Hispanic
        * Pac = Native Hawaiin and Pacific Islander alone, not Hispanic
        * Oth = Other race and two or more races, not Hispanic
        * Bl+ = Black alone or in combination with other races, including Hispanic
        * Nat+ = American Indian and Alaska native alone or in combination with other races, including Hispanic
        * Asn+ = Asian alone or in combination with other races, including Hispanic
        * Pac+ = Native Hawaiin and Pacific Islander alone or in combination with other races, including Hispanic
    * set =
        * tot = Total population
        * vap = voting age population

* For Election CSVs, <party>_<year>_<contest>, where
    * party =
        * Tot = total votes of all parties
        * Dem = Democratic Party
        * Rep = Republican Party
    * contest =
        * pres = President
        * sen = US Senate
        * gov = Governor
        * ltg = Lt. Governor
        * ag = Attorney General

