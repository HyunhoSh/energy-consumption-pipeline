# energy-consumption-pipeline
## Data Source

This project uses the "World Energy Consumption" dataset from Kaggle.

- Source: Kaggle  
- Dataset: World Energy Consumption
- Link: https://www.kaggle.com/datasets/pralabhpoudel/world-energy-consumption/data

The dataset is used for educational and non-commercial purposes only.

# Energy Consumption Pipeline with PySpark

This project demonstrates an end-to-end data and machine learning pipeline using PySpark in Databricks. The goal is to process energy consumption data and build a simple predictive model to support data-driven insights.

# Title: Predicting Greenhouse Gas Emissions Using Energy Data
## Project Overview
This project explores how energy consumption and economic factors relate to greenhouse gas emissions.
The goal was not only to build a predictive model, but also to understand which factors actually drive emissions and how reliable those relationships are.

The dataset includes country-level data from 2002 to 2018, covering energy usage (coal, oil, gas, renewables), GDP, population, and emissions.

## Problem Definition
- Target: Greenhouse Gas Emissions
- Features:
    1. Population
    2. GDP
    3. Coal, oil, gas and renewable energy consumption
    4. Lagged emissions (previous 1 and 2 years)

### Lagged emissions

- `emissions_lag1`: Emissions from the previous year  
- `emissions_lag2`: Emissions from two years prior  

These features allow the model to incorporate historical trends, as current emission levels are strongly influenced by past values.  
By including lag features, the model can better understand patterns over time rather than relying solely on current input variables.

## Data Preparation
