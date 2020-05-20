# baseline mortality
The baseline mortality database contains historical data about deaths in different countries (see below) as well as provisional numbers for 2020 for some countries.
Whenever possible, the cases are given on a daily basis and regional level.

## Data sources

Name | Country | [Code](https://www.nationsonline.org/oneworld/country_code_list.htm) | Source | Regional levels mapping | frequency
------|----------|---------|------|--------|--------|
UK-ONS | England and Wales | GBR  | https://www.ons.gov.uk/peoplepopulationandcommunity/birthsdeathsandmarriages/deaths/datasets/weeklyprovisionalfiguresondeathsregisteredinenglandandwales  | NUTS-1 region | weekly
BEL-STATBEL | Belgium | BEL | https://statbel.fgov.be/en/open-data/number-deaths-day-municipality | municipality (GADM-4) | daily
TUR-TUIK | Turkey | TUR | https://biruni.tuik.gov.tr/medas/ | NUTS-1 region | monthly
AUS-ABS | Australia | AUS | https://www.abs.gov.au/AUSSTATS/abs@.nsf/DetailsPage/3302.02018?OpenDocument | state or territory | monthly
DEU-DESTAT | Germany | DEU | https://www.destatis.de/DE/Themen/Gesellschaft-Umwelt/Bevoelkerung/Sterbefaelle-Lebenserwartung/Tabellen/sonderauswertung-sterbefaelle.html?nn=375478 | state (Bundesland) | daily
USA-CDC | USA | USA | https://wonder.cdc.gov/ | state | monthly
SWE-SCB | Sweden | SWE | https://www.scb.se/BE0101-en | county (län) | monthly
UN | Australia, Belgium, Brazil, Canada, Hong Kong, Macao, Egypt, France, Germany, Iran, Islamic Republic of, Ireland, Italy, Japan, Malaysia, Mexico, Netherlands, Pakistan, Philippines, Portugal, Korea, Republic of, Russian Federation, Spain, Sweden, Switzerland, Thailand, Turkey, United Kingdom, United States | AUS, BEL, BRA, CAN, HKG, MAC, EGY, FRA, DEU, IRN, IRL, ITA, JPN, MYS, MEX, NLD, PAK, PHL, PRT, KOR, RUS, ESP, SWE, CHE, THA, TUR, GBR, USA | http://data.un.org/Data.aspx?d=POP&f=tableCode%3A65 | n/a | monthly

## Schema for the table

Name | Data type | Short Description
------|------------|------------------
SOURCE | VARCHAR | Data source (see above)
DATE | DATE | Date of the statistics. For weekly and monthly statistics, the first day of the respective week/ month.
COUNTRY | VARCHAR | English name for the country
COUNTRYCODE | VARCHAR(3) | ISO 3166-1 alpha3 country code
region | VARCHAR | Region
gid | VARCHAR | GADM code of the region. A list of codes, if the region contains sesveral GADM regions.
DEATHS | INT | Number of deaths during the time period

## Data from the Economist repository

The Economist has collected similar data on github<sup>[1](#myfootnote1)</sup>. It is discussed in the article<sup>[2](#myfootnote2)</sup>.
We mirror the data from the `historical deaths` folder in our database, with gid information added.
Please refer to the readme of that project [here](https://github.com/TheEconomist/covid-19-excess-deaths-tracker/blob/master/README.md) for more details on the sources and the format.

______________________________________________________________________

<a name="myfootnote1">1</a>: James Tozer and Martín González: TheEconomist/covid-19-excess-deaths-tracker. GitHub repository available at https://github.com/TheEconomist/covid-19-excess-deaths-tracker, 2020.

<a name="myfootnote2">2</a>: Tracking covid-19 excess deaths across countries. In The Economist, 16 April, 2020. Available at https://www.economist.com/graphic-detail/2020/04/16/tracking-covid-19-excess-deaths-across-countries.