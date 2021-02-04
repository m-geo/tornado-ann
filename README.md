# tornado-ann
This repository contains a sample of code written for the project "Using Machine Learning to Predict Tornadoes Based on Sounding and Reanalysis Data" in the period between summer 2018 and fall 2020. This sample focuses on the sounding data portion of the project.

## storm_data
This is a folder with severe weather data downloaded from https://www.ncdc.noaa.gov/stormevents/ftp.jsp for the years 1973-2017, along with helper files that are used in data_analysis.ipynb to convert the event locations (given as county names in the NOAA data) to latitude and longitude coordinates

## sounding data
station_list.txt contains a list of all stations in the University of Wyoming Upper Air Soundings database (http://weather.uwyo.edu/upperair/sounding.html) that have continuous data collection over the 1973-2017 period. sounding_retrieval.sh will download all 12Z records from those stations in that time period to the ./data/ folder. It can be easily adjusted to also download 00Z.
data_analysis.ipynb contains the majority of the data processing and analysis functions used when dealing with the sounding data in this project.