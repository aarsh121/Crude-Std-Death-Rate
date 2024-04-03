**Objective**
This is project for 'Our world in Data' organization. In this we are calculating Crude death rate and age-standardized death rate due to COPD in America and Uganda for the year 2019.

**Data used are-**
World population data 2022, age group with 5 year interval-  United Nations
Age Standardization Table
COPD death rate for age groups for both countries.

In this data analysis excercise we are going to see Crude Death rate and Age Standardized Death rate. We have below assets at our disposal-

Population Exposure dataset from WHO('WPP2022_PopulationByAge5GroupSex_Medium'-5 July 2022)
Death rates of chronic obstructive pulmonary disease(COPD) of specific age for both countries.
A pdf which contains the WHO standard population data in Table-1.

**Data Processing-**

First we are going to load population dataset and filter it for USA and Uganda Population for 2019. We will create two new dataframes which will contain population data for USA and Uganda.
Saved COPD death rate in a csv.
Used Pdfplumber tool to extract the Table 1 from the WHO pdf. Table is at page-9.
We will clean the data if required.

**Methodologies-**

Now we have two seperate dataframes for each counrty(USA-df_am, Uganda-df_ugh). We will merge the COPD Death rates and WHO standard Population in both the dataframes.

After that we will calculate total death due to COPD for each specific age group using COPD death rate and Total Population.

Calculating crude rate for 100k population= (Total_deaths/Total_population)*100000

To calculate Age Standardized death rate - we will multiply each age specific death rate with WHO standard population proportion. and add them all. This will give us age adjusted death rate for the country.
