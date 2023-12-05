# CME538_2023
Group project for the University of Toronto's Fall 2023 CME538 course, published 2023-12-06

Written by Natalie Fylak, Katherine Westerlund, and Diana Zaraza Pena 

## The Problem at Hand 
The City of Toronto's transit system (the TTC), is notorious within the city for being [unreliable]([url](https://www.thestar.com/opinion/contributors/transit-in-toronto-has-never-felt-so-broken-it-s-time-for-the-ttc-board/article_4917e163-4ea2-58fa-9ba8-6fbcc5c685c9.html)) and [fundamentally flawed]([url](https://torontolife.com/deep-dives/who-broke-the-ttc-inside-torontos-public-transit-disaster/)https://torontolife.com/deep-dives/who-broke-the-ttc-inside-torontos-public-transit-disaster/). The general mistrust of the public transportation can drive people towards other modes of transportation (most notably, personal vehicle travel), which has the impact of further delaying road-based public transportation. 

Our objective was to understand how the delays and reliability of the TTC compared to other transit systems in Canada. Due to limitations in data availability, the city of Montreal's subway system and the city of Calgary's bus system were used to compare to their TTC counterparts.

## REQUIRED DATA
The TTC data was pulled from the City of Toronto's open data website (here: https://open.toronto.ca/catalogue/?search=ttc&sort=score%20desc). The Montreal STM data was pulled from the City of Montreal (here: https://donnees.montreal.ca/dataset/incidents-du-reseau-du-metro). The Calgary Transit data was pulled from the City of Calgary (here: https://data.calgary.ca/Transportation-Transit/Transit-Incident-Log/9m8z-ibsn). 

*The City of Calgary data must be downloaded directly from the website (linked above), as the file exceeds the maximum github file size*. 

Weather data was pulled from the Environment and Climate Change historical climate data database (here: https://climate.weather.gc.ca/historical_data/search_historic_data_e.html). 

API data (not used for final analysis) collection were performed on the following data sources: 
* OC Transportation GTFS-RT feed (key can be obtained here: https://www.octranspo.com/en/plan-your-trip/travel-tools/developers/) 
* Metrolinx's Go Network GTFS-RT feed (key can be obtained here: https://www.metrolinx.com/en/about-us/open-data)
* Translink's GTFS-RT feed (key can be obtained here: https://www.translink.ca/about-us/doing-business-with-translink/app-developer-resources/rtti) 
* STM's GTFS-RT feed (key can be obtained here: https://www.stm.info/en/about/developers) 

Python Requirements:
* Python v 3.11 (code may be compatible with previous python versions, however it has not been tested with such).
* Jupyter
* Pandas 
* Seaborn 
* Matplotlib 
* Numpy
* & others (see requirements.txt)

## METHODOLOGY
If intending to replicate the analysis conducted for CME 538: 
* First, start with the IMPORT_DATA and weather_files jupyter files.
*   These files will walk you through the process for compiling the weather data and transportation data for initial processing.
* Second, go to the EDA and Calgary_EDA files.
*   These files will walk you through the process for merging the weather and transportation data, cleaning the datasets, and provide some exploratory data analysis.
* Finally, check out the DataVisualizations jupyter file.
*   Here you will find more advanced EDA work for the TTC dataset, including information on peak vs offpeak delays. 

## RESULTS

The results can be seen within the EDA and DataVisualizations jupyter files. Here, a series of graphs show the trends & overall levels of delay in the different transit systems of interest. 

An in-depth discussion of the data analysis and results can be found on Medium here: <link>. 
