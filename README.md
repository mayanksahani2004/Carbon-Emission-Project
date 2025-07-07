# CARBON EMISSION PROJECT

## Problem Statement:
Analysis of country-specific data and development of machine learning models in order to predict CO2 emissions from country parameters. The project uses the publicly available dataset Climate Change Data from the World Bank Group, which provides data on the vast majority of countries over a range of years for parameters such as:

- country: the vast majority of countries worldwide
- year: ranging from 1990 to 2011
- various emissions of greenhouse gases such as CO2, CH4, N2O, others
- population-specific parameters: population count, urban population, population growth, etc.
- country economic indicators: GDP, GNI, Foreign Direct Investment, etc.
- land-related parameters: cereal yield, agricultural land, Nationally terrestrial protected areas, etc.
- climate data: precipitations, national disasters, etc.
- energy use
- counts of certain types of medical personnel

## WEEK 1 : Data Cleaning and Preparation

### Notebook Contents:
1. Introduction - project and notebook summary, notes on the data source
2. Notebook setup - libraries and data import
3. Global data overview
4. Definition of the initial project goals
5. Data cleaning
- dealing with missing values
- transformation of the columns into a numerical data type
- renaming of features
- removing empty columns and rows
6. Data frame transformation
- melting of the data for each variable
- integration of the data into a suitable data frame format
- Removal of missing values
- detection of missing values
- removal of missing values by filtering the columns and rows, so that minimal amount of features and rows are lost
7. Export the clean data frame to a file

### Data source
The used data comes from the Climate Change Data of the World Bank Group, which provides country-specific data on parameters such as CO2 emissions, energy use, population count, urban population, cereal yield, nationally terrestrial protected areas, GDP, GNI, etc.

The dataset is publicly available at https://datacatalog.worldbank.org/dataset/climate-change-data and licenced under the Creative Commons Attribution 4.0 International license.


## Week 2 – Data Exploration & Visualization
During Week 2, we conducted a comprehensive exploratory data analysis (EDA) of the cleaned dataset to understand underlying patterns, validate assumptions, and prepare for modeling.

### Goals:
Examine trends and relationships in carbon emissions data.
Identify impactful features for predictive modeling.
Detect multicollinearity and distribution issues.

### Key Highlights:

- Trend Analysis:
A time-series plot revealed a consistent rise in global CO₂ emissions per capita over the years, signaling growing carbon intensity worldwide.
The global per capita CO₂ emissions remained largely steady between 1991 and 2008, averaging ~4.6 metric tons.

- Population vs Emissions:
A scatter plot between total CO₂ emissions and population showed a strong positive relationship, reinforcing the role of population growth in emission trends.
The population size is a significant driver of total CO₂ emissions**. However, **emissions per person can vary widely**, as countries with similar populations show vastly different total CO₂ outputs

- Feature Engineering:
A new feature en_ttl (total energy use) was derived to capture aggregate energy consumption, enabling a more holistic understanding of energy-emission dynamics.

- Correlation Insights:
Heatmaps uncovered strong associations:
co2_ttl highly correlated with en_ttl.
co2_per_cap with en_per_cap.
Moderate positive links between gni_per_cap, cereal_yield, and emissions.

- Country-Level Analysis:
Country-wise comparison of emissions and urban population rates revealed that highly industrialized nations typically report higher per capita emissions.

- Outliers:
Another significant observation is the cluster of orange outlier points with CO₂ emissions per capita ranging between 25 and 40 metric tons, all attributed to the United Arab Emirates (ARE). While there are other country-specific outliers, they do not substantially impact the overall trend.

### Outcome:
The analysis helped identify key drivers of CO₂ emissions such as energy use, population size, urbanization, and economic output. Insights from this week will directly inform feature selection and model design in the upcoming stages.
