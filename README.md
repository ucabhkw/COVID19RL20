# COVID19RL20

This repository is for the paper (doi://).

## Folder "RAW" : 
The files in 'raw' are  ...
the time series data of confirmed, recovered, and deceased cases from Johns Hopkinsons Data Repository, and
population size, population density, medium-term population (15 to 65 years old), gross domestic product (GDP), geological information (longitude, latitude), and life expectancy obtained from official publications through the United Nations database, Wikipedia, and news.

 Data sources are as follows:   
#### (1) Index case date (date of the first confirmed patient) : 
 - Johns Hopkins coronavirus data repository : https://github.com/CSSEGISandData/COVID-19.
 - WHO’s case reports : https://www.who.int/emergencies/diseases/novel-coronavirus-2019.
 - Wikipedia : https://en.wikipedia.org/wiki/2019%E2%80%9320_coronavirus_pandemic.

(2) The number of test, confirmed infection, recovery and death : 
- Johns Hopkins coronavirus data repository : https://github.com/CSSEGISandData/COVID-19.
- WHO’s case reports : https://www.who.int/emergencies/diseases/novel-coronavirus-2019.
- Centers for Disease Control and Prevention’s reports : https://www.cdc.go.kr.
- OurworldInData Coronavirus Pandemic (COVID-19): https://ourworldindata.org/coronavirus.

(3) The timing and intensity of domestic lockdown and international travel restrictions : 
- Wikipedia : https://en.wikipedia.org/wiki/2019%E2%80%9320_coronavirus_pandemic.

(4) The population size, population density, population mid-year (aged 15 to 65 years old) : 
- Wikipedia : https://en.wikipedia.org/wiki/2019%E2%80%9320_coronavirus_pandemic.
- UN : https://data.un.org.
- WHO : https://www.who.int/.
- IHME (The Institute for Health Metrics and Evaluation): http://www.healthdata.org/.

(5) GDP : 
- Wikipedia : https://en.wikipedia.org/wiki/2019%E2%80%9320_coronavirus_pandemic.
- UN : https://data.un.org.
- IHME (The Institute for Health Metrics and Evaluation): http://www.healthdata.org/.

(6) Life expectancy :
- WHO : https://apps.who.int/gho/data/view.main.SDG2016LEXv?lang=en.

(7) Geological Information :
- Johns Hopkins coronavirus data repository : https://github.com/CSSEGISandData/COVID-19.
  
However, I would like to mention that unlike the timeline in which this study was conducted, it is now possible to collect this or more detailed and interesting data from the WHO site and some others (https://covid19.who.int/table, https://console.cloud.google.com/marketplace/browse?filter=category:covid19&rif_reserved).

2. Folder "Preprocessed" : 
The data includes all of the above. After merging all the tables, we adjusted the data to [0,1] and anonymized the country name.
Severitylevel is defined as the crude death rate due to COVID-19 reported on 7th April 2020 (See more details from the following paper doi://).
It is used as an indicator of the overall crisis severity level and divided into four levels.

3. Folder "Analysis" : 
The folder contains step-by-step analysis process.
As explained in the paper, we adapted and worked on the network in the previous papers, mainly tuning (https://github.com/darkefyre/sepsisrl/) for the network architecture.

We are grateful to all individuals who collect and share epidemiological data on COVID-19 outbreaks worldwide and for the excellent previous research available to us.
