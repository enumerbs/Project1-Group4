# Project Title: Uber Rides and Weather

## Team members (Group 4)
Zahra Razook,  Mary (Jiahui) Du, Isa Huseni, Greg Presneill

## Project Description
For this project, we will explore the ‘Uber Pickups in New York City’ data for 2014 available from Kaggle, and investigate what effect weather conditions had on ride demand (Uber usage).

## Summary and Conclusion

We found evidence of a mildly positive correlation between warmer weather and Uber demand, and no correlation correlation between precipitation (rain/snow/hail) events and Uber demand.

We further divided the temperature data into three groups - cold (less than 10 degrees), mild (between 10 and 25 degrees), and warm (above 25 degrees Celsius) - with a view to discovering if Uber usage increased on relatively cold or warm days. Analysis appeared to show a potential difference in the mean values of those groups, but a quantitative result could not be determined as the data in those groups was found not to be normally distributed (so ANOVA testing could not be applied). Intended analysis of potential changes in demand considering weather conditions at various times of day was not possible as the available weather data was at day (24 hour) resolution only.

In conclusion, we expected that more Uber trips would be taken in wet and cold weather, but we discovered evidence only for increased Uber usage in warmer weather.

## Project Folder Structure
```
./README.md (this file)
./Project1-Group4-Part1_EDA.ipynb
./Project1-Group4-Part2_TempAndRain_Analysis.ipynb
./Project1-Group4-Part3_SeasonsAndTimeOfDay_Analysis.ipynb
./group_presentation
./data
    /combined
    /kaggle_csv/uber-raw-data-2014
    /kaggle_sample
    /noaa_csv/2014
    /noaa_pdf/2014
```
- This README provides an overall description of the project and results.
- The three 'Project1-Group4' Jupyter notebooks describe and implement the data manipulation and analysis tasks undertaken to analyse the datasets and produce the results.
    - The first part represents initial Exploratory Data Analysis.
    - The second part contains the Uber usage verses Temperature and Rain conditions analysis.
    - The third part contains the Uber usage verses Season and Time of Day analysis.
- The 'group_presentation' subfolder contains our final presentation in PDF format.
- The 'data/combined' folder contains the combined weather data for New York City (Central Park) weather station for Apr-Sep 2014, after conversion to CSV format and data cleansing.
    - NOTE: the analysis Notebook also writes the combined Uber trips data file here as an intermediate step (but the combined file is not included in this repository due to its size).

- The 'data/kaggle_csv/uber-raw-data-2014' folder contains the six data files of Uber trips data for Apr-Sep 2014 after conversion to CSV format. (See further details below on the source of this data.)
- The 'data/kaggle_sample' folder provides a random sample of 100 rows from the combined Uber trips data.
- The 'data/noaa_csv/2014' folder contains the weather data converted to CSV, with 'T' (Trace) data points converted to zero values.
- The 'data/noaa_pdf/2014' folder contains the original weather data files for Apr-Sep 2014 in PDF format (See further details below on the source of this data.)

## Outline of Research Questions to Answer
1.	Correlation Analysis - How does weather affect the demand for Uber rides?
  - Is there a significant correlation between specific weather conditions (e.g., high or low temperatures, rain, snow) and the number of Uber rides?

2. Time-Based Analysis:
  - Are there seasonal trends in Uber usage that correlate with weather patterns?
  -	How does the time of day or day of the week impact Uber ride frequency in different weather conditions?

## Datasets to Be Used
- Uber rides Kaggle dataset (“Uber Pickups in New York City”)
  https://www.kaggle.com/datasets/fivethirtyeight/uber-pickups-in-new-york-city \
    Uber trip data from 2014:
    there are six files of raw data on Uber pickups in New York City from April to September 2014.

-	US National Oceanic and Atmospheric Administration (NOAA) for historical weather data
    https://www.ncdc.noaa.gov/cdo-web/datasets/GHCND/stations/GHCND:USW00094728/detail \
    Weather station: NY City Central Park, NY USA

## Rough Breakdown of Tasks
1.	Combine data from Uber ride data and Weather records
1.	Data cleaning and creating clean data frame.
1.	Analyze the Data
1.	Plot the Data
1.	Incorporate Statistics
1.	Summary for presentation
