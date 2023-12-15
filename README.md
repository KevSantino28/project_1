#   PROJECT 1 BOOTCAMP

##  PURPOSE

- "Thermal Trends and Crime Dynamics: Analyzing the correlation between Temperature Variations and Violent Crimes Reported in Chicago from 2012 to 2017".
- For the project, the data for the analysis used is from Kaggle and the Open-Meteo API.

##  CODE

- Python
- Packages:Pandas, Matplotlib, Spicy.stats, Numpy, Openmeteo_requests, Requests_Cache.

##  RESOURCES

- https://www.kaggle.com/code/umeshnarayanappa/exploring-chicago-crimes-2012-2016
- https://open-meteo.com/en/docs/historical-weather-api](https://archive-api.open-meteo.com/v1/archive"

##  PROJECT PLANNING

Analyze the correlation between Temperature Variations and Violent Crimes Reported in Chicago using Kaggle data and The Historical Weather API.

###  1-DATA ACQUISITION

The data used to do the analysis is an CSV file downloaded from kaggle.

###  2-SETUP THE OPEN-METEO API

Following setup the open-meteo steps are applied:
  - List the required variables.
  - Process the first location and use for loop to multiple locations or weather models.

![1](https://github.com/KevSantino28/project_1/assets/145527812/bb791a5f-80d4-4c22-90dd-a7329be23c3f)

  - Process daily data,
  - Renaming Date column.

###  3-DATA CLEANNING UP

  - Study the files, reading the CSV, read the crime data to analysis.
  - Check if the data have duplicates searching from the ID and blank columns.
  - List the Type of Crimes and number of reports from 2012 to 2017.

![2](https://github.com/KevSantino28/project_1/assets/145527812/bff4a207-1d17-43f3-97a7-eb2b17d98e12)

  - Clean up the columns.
  - Filter out the columns of crimes to show only the violent crimes defined as "ASSAULT, BATTERY, CRIM SEXUAL ASSAULT, OR HOMICIDE.
  - Formating the Date.
  - Merge the Open-Meteo API data and the CSV cleanned data.
  - Group by year and type the crimes filtered.

![3](https://github.com/KevSantino28/project_1/assets/145527812/6751218c-3adc-494b-ace3-9a659f1b3972)

### 4-ANALYZE THE DATA USING CHARTS

  - Use the Pie chart to show the overall percent of the Violent crimes from 2012 to 2017, and five chart pie addtionals showing the percent of the violent crimes for each year.
  - Utilize the Scatter chart to show the correlation weather vs report crimes from 2012 to 2017.

![5](https://github.com/KevSantino28/project_1/assets/145527812/b73b9b76-bf5d-4a52-a785-05ed2e2b4fa8)

  - Use the Bar chart to analyze the Crimes Committed per Tempemperature.
  - And to finish using the scatter chart to show th correlation between temperature and number of crimes for each each year between 2012 and 2017.

![Untitled](https://github.com/KevSantino28/project_1/assets/145527812/27e694b1-0726-40ce-a563-bf16f3c17113)


###  5-CONCLUSION

  - The conclusion of the analyses will be demonstrate in an presetation on the class using an powerpoint presentation.

    


