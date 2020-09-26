# Beijing-Multi-Site-Air-Quality

## Introduction
Air pollution refers to the release of pollutants into the air that are detrimental to human health and the planet as a whole. It has been proven through studies that air pollution directly affects the temperature of a location. Energy production and transportation are one of the major causes of air pollution. The burning of fossil fuels leads to release of various harmful and hazardous chemicals into the atmosphere. These chemicals along with pressure, wind, altitude and oceanic movement affect the temperature of a specific location. The main aim of this project is to analyze the relation between temperature and concentration of some of these pollutants in the atmosphere. Moreover, this project also emphasizes on the importance of Feature Creation in Data Mining.

## Objective
The main objective of this project is to predict the PM 2.5 levels in the air to determine the Air quality of Beijing.

## Problem description

To predict the PM 2.5 levels in the air to determine the Air quality of Beijing. There are multiple datasets concerning different districts in Beijing. The data was recorded hourly for each district.
 
## Data Description
This data set includes hourly air pollutants data from 12 nationally-controlled air-quality monitoring sites. The air-quality data are from the Beijing Municipal Environmental Monitoring Center. The meteorological data in each air-quality site are matched with the nearest weather station from the China Meteorological Administration. The time period is from March 1st, 2013 to February 28th, 2017. Missing data are denoted as NA.

The features in this dataset are provided as following

1.No: row number
2.year: year of data in this row
3.month: month of data in this row
4.day: day of data in this row
5.hour: hour of data in this row
6.PM2.5: PM2.5 concentration (ug/m^3)
7.PM10: PM10 concentration (ug/m^3)
8.SO2: SO2 concentration (ug/m^3)
9.NO2: NO2 concentration (ug/m^3)
10.CO: CO concentration (ug/m^3)
11.O3: O3 concentration (ug/m^3)
12.TEMP: temperature (degree Celsius)
13.PRES: pressure (hPa)
14.DEWP: dew point temperature (degree Celsius)
15.RAIN: precipitation (mm)
16.wd: wind direction
17.WSPM: wind speed (m/s)
18.station: name of the air-quality monitoring site

Size of the Dataset:
Number of attributes (columns) = 18
Number of data samples (rows) / region = 
Number of Regions: 12
Total Instances = 18 * 35064 * 12 = 7,573,824

## Data Preprocessing
### Appending Data
The data was given in form of 12 excel files. We used pandas to merge these 12 files into one dataframe and gave column names wherever necessary.
### Null Data
These types of data are not tolerable for applying any kind of machinelearning models. Analysis of a dataset which contains such data will result in prediction
with high error and very less accuracy. Hence, null data entities are found out and are replaced by the mean value of the respective attribute values. By doing so, the entire data set will remain balanced.
