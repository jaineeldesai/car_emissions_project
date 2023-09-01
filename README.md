# Project: Exploratory Data Analysis of CO2-Emissions of all new registered passenger cars in Germany in 2022

The Regulation (EU) No 2019/631 requires European Countries to record information for each new passenger car registered in its territory. Every year, each Member State shall submit to the Commission all the information related to their new registrations. In particular, the following details are required for each new passenger car registered: manufacturer name, type approval number, type, variant, version, make and commercial name, specific emissions of CO2 (NEDC and WLTP protocols), masses of the vehicle, wheel base, track width, engine capacity and power, fuel type and mode, eco-innovations and electricity consumption.

Under conditions defined by EU law, the WLTP laboratory test is used to measure fuel consumption and CO2 emissions from passenger cars, as well as their pollutant emissions.

Passenger cars and vans ('light commercial vehicles') are respectively responsible for around 12% and 2.5% of total EU emissions of carbon dioxide (CO2), which is the main greenhouse gas.

** NEDC- New European Driving Cycle (Excluded since 2021)
** WLTP- Worldwide Harmonised Light Vehicle Test Procedure

## Target levels
The EU fleet-wide CO2 emission targets set in the Regulation are as follows:

2020 to 2024
Cars: 95 g CO2/km
Vans: 147 g CO2/km
These target levels refer to the NEDC emission test procedure.

Since 2021, the emission targets for manufacturers are based on the WLTP.

## Motivation

To check if the emissions from the new registered cars is in the target level as well as compare with previous year to find any changes.
Also, to build a regression model to predict emissions based on several important parameters.

## Data Source 

The car emission data used for the analysis and model is collected from:
https://www.eea.europa.eu/en

## Exploratory Data Analysis

The exploratory data anaylsis is carried out in tableau and can be found here:
https://public.tableau.com/views/car_emissions_germany_2022/intro?:language=en-US&:display_count=n&:origin=viz_share_link

## Coding

### Cleaning Data
In the notebook 'cleaning_data.ipynb', the collected dataset 'data.csv'  is imported (which is available in the zip file).
The data is cleaned and stored to a MySQL database as well as a csv 'clean_car_data.csv' (also available in the same zip file).

### Regression Model

In the notebook 'emissions_model.ipynb', the 'clean_car_data.csv' is imported and the following steps are carried on:

* Data Exploration and Cleaning (based on the target)
* X-y Split
* Checking correlation
* Train-Test Split, Separating Numerical/Categorical, Transforming/Encoding Data
* Building Model and Making Predictions
* Model Assessment


