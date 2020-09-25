# COVID19RL20

- Folder "RAW" : 
The files in 'raw' are 
1) the time series data of confirmed, recovered, and deceased cases from Johns Hopkinsons Data Repository, and
2) population size, population density, medium-term population (15 to 65 years old), gross domestic product (GDP), geological information (longitude, latitude), and life expectancy obtained from official publications through the United Nations database, Wikipedia, and news.
However, I would like to mention that unlike the timeline in which this study was conducted, it is now possible to collect this or more detailed and interesting data from the WHO site.
(https://covid19.who.int/?gclid=CjwKCAjwh7H7BRBBEiwAPXjadmevUeNji5pXVlH3sVnnIE70wSOsN4-EqkQ_DEAeU6sZK2hohUkySxoC2OwQAvD_BwE).

- Folder "Preprocessed" : 
The data includes all of the above. After merging all the tables, we adjusted the data to [0,1] and anonymized the country name.
Severitylevel is defined as the crude death rate due to COVID-19 reported on 7th April 2020 (See more details from the following paper doi://).
It is used as an indicator of the overall crisis severity level and divided into four levels (low/medium/high/critical level of severity).

- Folder "Analysis" : 
The folder contains step-by-step analysis process.
As explained in the paper, we adapted and worked on the network in the previous papers, mainly tuning (https://github.com/darkefyre/sepsisrl/) for the network architecture.

We are grateful to all individuals who collect and share epidemiological data on COVID-19 outbreaks worldwide and for the excellent previous research available to us.
