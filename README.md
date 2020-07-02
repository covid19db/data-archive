# Oxford COVID-19 (OxCOVID19) Data Repository 

**OxCOVID19 Database** is a large, single-centre, multimodal database consisting of information relating to COVID-19 pandemic. 

**OxCOVID19 Project** [https://covid19.eng.ox.ac.uk/](https://covid19.eng.ox.ac.uk/)  aims to increase our understanding of the Covid-19 pandemic and elaborate possible strategies to reduce the impact on the society through the combined power of Statistical and Mathematical Modelling, and Machine Learning techniques.

The data contained in this repository is automatically generated by our system. It represents a dump of the database in comma-separated values (CSV).
Files are grouped in three folders:

- data-epidemiology: contains epidemiological data like the number of confirmed cases or deaths.
- data-government-response: contains data collected from the [Coronavirus Government Response Tracker](https://www.bsg.ox.ac.uk/research/research-projects/coronavirus-government-response-tracker).
- data-mobility: contains data related to mobility of population, as collected, for example, through mobile phones.
- data-statistics: contains general statistics about the countries and regions.

Each file contained in these folder is related to a different source. The list of sources is available at [this link](https://covid19.eng.ox.ac.uk/data_sources.html). The structure of each file and the meaning of each column are described in [this webpage](https://covid19.eng.ox.ac.uk/data_schema.html) for detailed explanations.

A summary of the available data is provided here:

Epiedmiology:

| File    | Country | Source | Features  | Terms of use |
|---------|---------|--------|-----------|--------------|
| AUS_C1A | Australia | [covid-19-au](https://github.com/covid-19-au/covid-19-au.github.io) | tested, confirmed, dead,recovered, hospitalised, hospitalised_icu | [For educational and academic research purposes](https://github.com/covid-19-au/covid-19-au.github.io) | 
| BEL_WY | Belgium |  | confirmed, recovered, dead, hospitalised, hospitalised_icu | | 
| BRA_MSHM | Brazil | [covid19-Brazil-timeseries](https://github.com/elhenrico/covid19-Brazil-timeseries) | confirmed (country-level), dead (country-level, adm_area_1) | [public domain](https://github.com/elhenrico/covid19-Brazil-timeseries/blob/master/README.md#public-domain-and-open-data) | 
| CAN_GOV | Canada | [Public Health Canada](https://www.canada.ca/en/public-health.html) | tested, confirmed, dead, recovered | [Attribution required](https://www.canada.ca/en/transparency/terms.html) | 
| CHE_OPGOV | Switzerland | [Kanton Zürich Statistisches Amt](https://github.com/openZH/covid_19) | confirmed, dead, hospitalised, hospitalised_icu | | 
| CHN_ICL | China | [Imperial College London, MRC Centre for Global Infectious Disease Analysis](https://github.com/mrc-ide/covid19_mainland_China_report) | confirmed, dead, hospitalised, hospitalised_icu | CC BY NC ND 4.0 |
| DEU_JPGG | Germany | [Jan-Philip Gehrcke (Gesundheitsaemter)](https://github.com/jgehrcke/covid-19-germany-gae) | confirmed, dead | [MIT](https://github.com/jgehrcke/covid-19-germany-gae/blob/master/LICENSE) |
| ESP_MS | Spain | [Ministerio de Sanidad](https://www.mscbs.gob.es/profesionales/saludPublica/ccayes/alertasActual/nCov-China/situacionActual.htm) | confirmed, dead, hospitalised, hospitalised_icu | ["Desnaturalización" prohibited, citation required](https://www.mscbs.gob.es/avisoLegal/home.htm) |
| ESP_MSVP | Spain | [Victor Vincente Palacios](https://raw.githubusercontent.com/victorvicpal/COVID19_es/master/data/final_data/dataCOVID19_es.csv) | confirmed, recovered, dead, hospitalised, ICU | [Apache License 2.0](https://github.com/victorvicpal/COVID19_es/blob/master/LICENSE) |
| EU_ZH | Europe | [COVID19 EU](https://github.com/covid19-eu-zh/covid19-eu-data) | tested, confirmed,  dead, recovered, hospitalised, hospitalised_icu | [MIT](https://github.com/covid19-eu-zh/covid19-eu-data/issues/57) |
| FRA_SPF | France | [Santé publique France](https://www.data.gouv.fr/fr/datasets/donnees-hospitalieres-relatives-a-lepidemie-de-covid-19/) | recovered, dead, hospitalised, hospitalised_icu | [License Ouverte/Open License 2.0](https://www.data.gouv.fr/fr/datasets/donnees-hospitalieres-relatives-a-lepidemie-de-covid-19/) |
| FRA_SPFCG | France | [Cédric Guadalupe (Agence Regionale de Sante and others)](https://github.com/cedricguadalupe/FRANCE-COVID-19) | recovered, dead, hospitalised, hospitalised_icu | [GPL 3.0](https://github.com/cedricguadalupe/FRANCE-COVID-19/blob/master/LICENSE) |
| GBR_PHE | UK - England | [Public Health England](https://coronavirus.data.gov.uk/) | tested, confirmed, dead | [Open Government Licence v3.0](https://www.nationalarchives.gov.uk/doc/open-government-licence/version/3/) |
| GBR_PHTW | UK | [Tom White](https://github.com/tomwhite/covid-19-uk-data) | tested, confirmed, dead | [The Unlicense](https://github.com/tomwhite/covid-19-uk-data/blob/master/LICENSE.txt) |
| GBR_PHW | UK - Wales | [Public Health Wales](https://public.tableau.com/profile/public.health.wales.health.protection#!/vizhome/RapidCOVID-19virology-Public/Headlinesummary) | tested, confirmed, dead | [Open Government Licence v3.0](https://www.nationalarchives.gov.uk/doc/open-government-licence/version/3/) |
| IDN_GTPPC | Indonesia | [COVID19.go](https://covid19.go.id/) | confirmed, recovered, dead | Standard "all rights reserved" notice. No licensing information. |
| IND_COVIND | India | [COVID19india](https://api.covid19india.org/) | tested, confirmed, recovered, dead | [GPL 3.0](https://github.com/covid19india/api/blob/master/LICENSE) |
| IRL_HSPC | Ireland |  | confirmed |  |
| ITA_PC | Italy | [Protezione Civile](https://github.com/pcm-dpc/COVID-19) | tested, confirmed, recovered, dead, hospitalised, ICU, quarantined | [CC BY 4.0](https://github.com/pcm-dpc/COVID-19/blob/master/LICENSE) |
| ITA_PCDM | Italy | [Davide Magno (Protezione Civile)](https://github.com/DavideMagno/ItalianCovidData) | tested, confirmed,  dead, recovered, hospitalised, ICU, quarantined | [CC0 1.0 Universal](https://github.com/DavideMagno/ItalianCovidData/blob/master/LICENSE) |
| JPN_C1JACD | Japan | [code4sabae/covid19s](https://github.com/code4sabae/covid19) | tested, confirmed, recovered, dead, hospitalised, hospitalised_ic | [CC BY](https://github.com/code4sabae/covid19) |
| KOR_DS4C | South Korea | [Jihoo-Kim](https://github.com/jihoo-kim/Data-Science-for-COVID-19) | tested, confirmed, recovered, dead | [CC BY-NC-SA 4.0](https://github.com/jihoo-kim/Data-Science-for-COVID-19) |
| LAT_DSRP | South Korea | [Jihoo-Kim](https://github.com/jihoo-kim/Data-Science-for-COVID-19) | tested, confirmed, recovered, dead | [CC BY-NC-SA 4.0](https://github.com/jihoo-kim/Data-Science-for-COVID-19) |
| MYS_MHYS | Malaysia | [Young Sung](https://github.com/ynshung/covid-19-malaysia) | confirmed, dead, hospitalised | [Public Domain](https://github.com/ynshung/covid-19-malaysia/blob/master/LICENSE) |
| NGA_CDC | Nigeria | [covidnigeria.herokuapp.com](https://covidnigeria.herokuapp.com/) | confirmed, recovered, dead |  |
| NGA_SO | Nigeria | [Young Sung](https://github.com/ynshung/covid-19-malaysia) | confirmed, recovered, dead |  |
| NLD_CW | Netherlands | [CoronaWatchNL](https://github.com/J535D165/CoronaWatchNL/tree/master/data) | confirmed, dead, hospitalised | [CC0](https://github.com/J535D165/CoronaWatchNL) |
| NLD_WY | Netherlands |  | confirmed, dead, hospitalised | |
| PAK_GOV | Pakistan | [National Information Technology Boards](https://datastudio.google.com/u/0/reporting/1PLVi5amcc_R5Gh928gTE8-8r8-fLXJQF/page/kyNJB) | confirmed,  dead, recovered |  |
| POL_WIKI | Poland | [Wikipedia](https://en.wikipedia.org/wiki/2020_coronavirus_pandemic_in_Poland) | confirmed, dead | [CC0](https://www.wikidata.org/wiki/Wikidata:Licensing) |
| PRT_MSDS | Portugal | [dssg-pt](https://github.com/dssg-pt/covid19pt-data) | tested, confirmed, recovered, dead, hospitalised, ICU, quarantined | [MIT](https://github.com/dssg-pt/covid19pt-data) |
| RUS_GOV | Russia |  | confirmed, recovered, dead | |
| SWE_GM | Sweden | [Elin Lütz](https://github.com/elinlutz/gatsby-map/tree/master/src/data/time_series) | confirmed, dead, adm_area_1 | [MIT](https://github.com/elinlutz/gatsby-map/blob/master/LICENSE) |
| SWE_SIR | Sweden | [SIR](https://portal.icuregswe.org/siri/report/corona.inrapp) | hospitalised_icu | [SIR Copyright](https://www.icuregswe.org/en/data--results/data-output-portal/) |
| THA_STAT | Thailand | [Department of Disease Control](https://covid19.th-stat.com/en/api) |confirmed, recovered, dead, hospitalised | [DGA Open Government License](https://data.go.th/en/dataset/covid-19-daily) |
| TUR_MHOE | Turkey | [Turkish Ministry of Health](https://covid19.saglik.gov.tr/) | tested, confirmed, dead, recovered, hospitalised_icu | [MIT](https://github.com/ozanerturk/covid19-turkey-api/blob/master/LICENSE) |
| USA_CTP | United States | [COVID Tracking Project](https://covidtracking.com/api) | confirmed, dead | [CC BY-NC-4.0](https://covidtracking.com/license) |
| USA_NYT | United States | [The New York Times](https://github.com/nytimes/covid-19-data) | confirmed, dead | [Attribution required, non-commercial use](https://github.com/nytimes/covid-19-data/blob/master/LICENSE) |
| WRD_ECDC | World | [European Centre for Disease Prevention and Control](https://www.ecdc.europa.eu/en/publications-data/download-todays-data-geographic-distribution-covid-19-cases-worldwide) | confirmed, dead, recovered | [https://www.ecdc.europa.eu/en/copyright](ECDC Copyright) |
| WRD_WHO | World | [WHO](https://covid19.who.int/) | confirmed, recovered, dead |  |
| ZAF_DSFSI | South Africa | [Data Science for Social Impact research group, University of Pretoria](https://github.com/dsfsi/covid19za) | tested, confirmed, recovered , dead, hospitalised, hospitalised_icu, quarantined  | [MIT](https://github.com/dsfsi/covid19za/blob/master/LICENSE) |


---

__Cite as:__ Adam Mahdi, Piotr Błaszczyk, Paweł Dłotko, Dario Salvi, Tak-Shing Chan, John Harvey, Davide Gurnari, Yue Wu, Ahmad Farhat, Niklas Hellmer, Alexander Zarebski, Lionel Tarassenko,
<em>Oxford COVID-19 Database: multimodal data repository for understanding the global impact of COVID-19. University of Oxford</em>, 2020.

---



