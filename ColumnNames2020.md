## Column Names in CSV files

For 2020 VTD Shapes, the first two CSV Columns are GEOID20 and Name (name of the VTD).
Subsequent CSV Column Headings are in the form "Category_Year_Dataset[_Modifier]_Field".

* Category
    * T = Total Population
    * V = Voting Age Population
    * E = Elections
* Year = 2-digit year
* Demographic Data (number of persons)
    * Dataset (including modifiers)
        * CENS = Total Population from the decennial census
        * CENS_ADJ = Total Population from the decennial census, Adjusted for incarcerated persons
        * ACS = Total Population from the 5-year American Community Survey estimate
        * VAP = Voting Age Population with Race Combination categories from the decennial census
        * VAP_NH = Voting Age Population with Non-Hispanic Race Alone categories from the decennial census
        * CVAP = Citizen Voting Age Population based on the 5-year American Community Survey estimate
    * Field
        * Total = Total persons
        * White = White alone, not Hispanic
        * Hispanic = All Hispanics regardless of race
        * Black = Black alone or in combination with other races, including Hispanic
        * Asian = Asian alone or in combination with other races, including Hispanic
        * Native = American Indian and Alaska Native alone or in combination with other races, including Hispanic
        * Pacific = Native Hawaiian and Pacific Islander alone or in combination with other races, including Hispanic
        * BlackAlone = Black alone, not Hispanic
        * AsianAlone = Asian alone, not Hispanic
        * NativeAlone = American Indian and Alaska Native alone, not Hispanic
        * PacificAlone = Native Hawaiian and Pacific Islander alone, not Hispanic
        * OtherAlone = Other race alone, not Hispanic
        * TwoOrMore = Two or more races, not Hispanic
        * RemTwoOrMore = Remainder of two or more races, not Hispanic (for CVAP only because it does not include some race combinations already included other fields)
* Election Data (number of votes)
    * Dataset
        * COMP = DRA's Composite
        * PRES = President
        * SEN = U.S. Senator
        * GOV = Governor
        * AG = Attorney General
        * AUD = Auditor
        * LTG = Lieutenant Governor
        * SOS = Secretary of State
        * TREAS = Treasurer
        * SC* = State Supreme Court (with seat designation)
        * CONG = U.S. Congress
    * Modifier
        * ROFF = Runoff election
        * SPEC = Special election
        * SPECROFF = Special Runoff election
    * Field
        * Tot = Total votes
        * Dem = Democratic votes
        * Rep = Republican votes
