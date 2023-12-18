#   PROJECT 1 BOOTCAMP

##  PURPOSE

- "Thermal Trends and Crime Dynamics: Analyzing the correlation between Temperature Variations and Violent Crimes Reported in Chicago from 2012 to 2017".
- For the project, the data for the analysis used is from Kaggle and the Open-Meteo API.

##  CODE

- Python
- Packages:Pandas, Matplotlib, Spicy.stats, Numpy, Openmeteo_requests, Requests_Cache.

##  PROJECT PLANNING

Analyze the correlation between Temperature Variations and Violent Crimes Reported in Chicago using Kaggle data and The Historical Weather API.

Per Corcoran and Zahnow in their metadata analysis, 79% of studies of this relationship define violent crime as: 
“...a category that includes rape and sexual assault, robbery, assault, crimes against the person and murder.” [3]

We defined violent crime as the following: instances of assault, battery, criminal sexual assault, and homicide.
We fit Corcoran and Zahnow's definition to our crime dataset tags.

Alternative Hypothesis: If it is hotter outside, then there will be more instances of violent crime.
Null Hypothesis: The weather outside has no impact on the prevalence of violent crime.

We believe the relationship between temperature variation and violent crime is more nuanced than correlation/causation: violent crime is 
a complex amalgam of socio-economic and psychological factors. Drawing a clear causation relationship would be tenuous at best,
so we're exploring it as correlation and either indirect causation or direct causation.

Indirect causation: If it’s hotter outside, more people will be outside – leading to more crime being committed.
Direct causation: If it’s hotter outside, people will suffer greater psychological effects of heat – causing more crime being committed.

Indirect causation would see instances of violent crime plateau at a certain temperature. Direct causation would see the temperature and instances of violent crime increase linearly.

Ultimately, our hypothesis is one of indirect causation.


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

  - Use the Pie chart to show the overall percent of the Violent crimes from 2012 to 2017, and five chart pie additionals showing the percent of the violent crimes for each year.
  - Utilize the Scatter chart to show the correlation weather vs report crimes from 2012 to 2017.

![5](https://github.com/KevSantino28/project_1/assets/145527812/b73b9b76-bf5d-4a52-a785-05ed2e2b4fa8)

  - Use the Bar chart to analyze the Crimes Committed per Tempemperature.
  - And to finish using the scatter chart to show th correlation between temperature and number of crimes for each each year between 2012 and 2017.

![Untitled](https://github.com/KevSantino28/project_1/assets/145527812/27e694b1-0726-40ce-a563-bf16f3c17113)


###  5-CONCLUSION

  - The primary conclusion of the analyses will be discussed in a presetation in class using a powerpoint presentation.

We’ve demonstrated a positive correlation and indirect causation relationship between the weather and instances of violent crime: as it gets hotter, there is more violent crime.

Our results plateau, with most instances occurring in the high 70s range.

Our ANOVA results show an extremely strong correlation, with a p-value of 0.0


###  RESOURCES

[1] Weather Data API
  Zippenfenig, P. (2023). Open-Meteo.com Weather API [Computer software]. Zenodo. https://doi.org/10.5281/ZENODO.7970649

  Hersbach, H., Bell, B., Berrisford, P., Biavati, G., Horányi, A., Muñoz Sabater, J., Nicolas, J., Peubey, C., Radu, R., Rozum, I., Schepers, D., Simmons, A., Soci, C., Dee, D., Thépaut, J-N. (2023). ERA5 hourly data on single levels from 1940 to present [Data set]. ECMWF. https://doi.org/10.24381/cds.adbb2d47

  Muñoz Sabater, J. (2019). ERA5-Land hourly data from 2001 to present [Data set]. ECMWF. https://doi.org/10.24381/CDS.E2161BAC

  Schimanke S., Ridal M., Le Moigne P., Berggren L., Undén P., Randriamampianina R., Andrea U., Bazile E., Bertelsen A., Brousseau P., Dahlgren P., Edvinsson L., El Said A., Glinton M., Hopsch S., Isaksson L., Mladek R., Olsson E., Verrelle A., Wang Z.Q. (2021). CERRA sub-daily regional reanalysis data for Europe on single levels from 1984 to present [Data set]. ECMWF. https://doi.org/10.24381/CDS.622A565A

  https://open-meteo.com/en/docs/historical-weather-api](https://archive-api.open-meteo.com/v1/archive

[2] Crime Data CSV
  Umeshnarayanappa, U. (2017, March 2). Exploring chicago crimes 2012-2016. Kaggle. https://www.kaggle.com/code/umeshnarayanappa/exploring-chicago-crimes-2012-2016 

[3] Metadata Analysis
  Corcoran, J., Zahnow, R. Weather and crime: a systematic review of the empirical literature. Crime Sci 11, 16 (2022). https://doi.org/10.1186/s40163-022-00179-8

[4] 2012 Discussion
  Davey, M. (2012, June 26). Rate of killings rises 38 percent in Chicago in 2012. The New York Times. https://www.nytimes.com/2012/06/26/us/rate-of-killings-rises-38-percent-in-chicago-in-12.html 

[5] District Map
  Consortium on Chicago School Research. (n.d.-a). Selected indicators from the U.S. Census and Chicago Public Schools Records related to the lives and schooling of children. https://consortium.uchicago.edu/web_reports/Schoolageenvironment/mainmap.htm 

[6] Poverty Map
  xhan20. (2013, September 9). Collection of poverty maps of Chicago. Data Model Prototype. https://datamodelprototype.wordpress.com/2013/09/09/collection-of-poverty-maps-of-chicago/ 

[7] AC in Public Housing
Gorner, J. (2023, March 24). Spurred by heat deaths of seniors in Rogers Park, Illinois Senate passes measure requiring AC at state-funded affordable housing. Chicago Tribune. https://www.chicagotribune.com/politics/ct-illinois-affordable-housing-ac-requirement-20230324-p6nn3o6ot5e35afraykeihkcim-story.html 

    


