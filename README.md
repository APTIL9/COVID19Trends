## In-depth Analysis of Global COVID-19 Trends

This repository contains datasets and SQL scripts for analyzing time-series data related to the COVID-19 pandemic. The analysis includes data cleaning, data transformation, and various descriptive statistics to understand the trends and patterns in the COVID-19 data.

### Overview

The project uses a time-series dataset of COVID-19 cases, which includes the number of confirmed cases, deaths, and recoveries, along with geographical information. The provided SQL scripts perform a detailed analysis on this dataset, including handling missing values, extracting basic statistics, and aggregating data at different levels.

### Files

#### 1. `data_time_series_covid19.xlsx`

This Excel file contains the time-series data related to COVID-19 cases, including:
- **Province**: The province or state within the country/region.
- **Country/Region**: The country or region where the data is reported.
- **Latitude**: The latitude of the location.
- **Longitude**: The longitude of the location.
- **Date**: The date of the data entry.
- **Confirmed**: The number of confirmed COVID-19 cases.
- **Deaths**: The number of deaths due to COVID-19.
- **Recovered**: The number of recovered COVID-19 cases.

#### 2. `SQL for analysing Covid data.sql`

This SQL file contains a series of SQL commands and comments that describe various steps for analyzing the COVID-19 data, including:

- **Database Creation and Selection**: Creating and selecting the `COVID` database for analysis.
- **Data Cleaning**: Checking and updating NULL values in the dataset.
- **Descriptive Statistics**: Performing basic statistical analysis, such as counting rows, grouping, and ordering data, and finding the minimum and maximum of confirmed, deaths, and recovered cases per month.

### Analysis and Conclusions

Based on the provided dataset and SQL analysis, the following conclusions have been drawn:

1. **Dataset Composition**: The dataset contains \(140,484\) rows, covering the period from January 22, 2020, to June 13, 2021.

2. **Data Variability**: The number of rows varies each month, indicating different levels of data reporting or availability across months. 

3. **Case Variations**: 
   - The minimum number of confirmed, deaths, and recovered cases is \(0\) for each month.
   - The maximum number of confirmed cases in a month reached \(823,225\) in December 2020.
   - The maximum number of deaths in a month reached \(7,374\) in June 2021.
   - The maximum number of recovered cases in a month reached \(1,123,456\) in December 2020.

4. **Conclusions**: 
   - The dataset provides a comprehensive view of the COVID-19 cases from January 2020 to June 2021.
   - The variability in the number of rows each month is likely due to differences in data reporting or availability.
   - The presence of zero minimum cases every month suggests that the dataset includes regions that did not report any cases in certain months.
   - The increasing trend in the maximum number of confirmed and recovered cases over the months indicates the varying impacts and responses to the pandemic in different regions over time.

### How to Run

1. **Load the Dataset**: Load the `data_time_series_covid19.xlsx` file into your SQL database under the table name `dbo.Data`.
2. **Execute SQL Scripts**: Run the SQL commands in the `SQL for analysing Covid data.sql` file sequentially to perform the analysis on the loaded dataset.
