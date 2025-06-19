CARBON EMISSION PROJECT

Problem Statement:
Analysis of country-specific data and development of machine learning models in order to predict CO2 emissions from country parameters. The project uses the publicly available dataset Climate Change Data from the World Bank Group, which provides data on the vast majority of countries over a range of years for parameters such as:

country: the vast majority of countries worldwide
year: ranging from 1990 to 2011
various emissions of greenhouse gases such as CO2, CH4, N2O, others
population-specific parameters: population count, urban population, population growth, etc.
country economic indicators: GDP, GNI, Foreign Direct Investment, etc.
land-related parameters: cereal yield, agricultural land, Nationally terrestrial protected areas, etc.
climate data: precipitations, national disasters, etc.
energy use
counts of certain types of medical personnel
etc.
The project is divided into two stages:

Data cleaning and preparation
Data exploration and Predictive analysis
Each of the stages is described in a separate Jupyter Notebook(.ipynp file) and a derived pdf file.

Stage 1: Data cleaning and preparation
Notebook Contents:
Introduction - project and notebook summary, notes on the data source
Notebook setup - libraries and data import
Global data overview
Definition of the initial project goals
Data cleaning
dealing with missing values
transformation of the columns into a numerical data type
renaming of features
removing empty columns and rows
Data frame transformation
melting of the data for each variable
integration of the data into a suitable data frame format
Removal of missing values
detection of missing values
removal of missing values by filtering the columns and rows, so that minimal amount of features and rows are lost
Export the clean data frame to a file
Data source
The used data comes from the Climate Change Data of the World Bank Group, which provides country-specific data on parameters such as CO2 emissions, energy use, population count, urban population, cereal yield, nationally terrestrial protected areas, GDP, GNI, etc.

The dataset is publicly available at https://datacatalog.worldbank.org/dataset/climate-change-data and licenced under the Creative Commons Attribution 4.0 International license.
