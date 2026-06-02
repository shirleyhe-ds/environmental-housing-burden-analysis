# environmental-housing-burden-analysis
Predicting socioeconomic status from environmental variables

## Overview
This project investigates the relationship between environmental pollution indicators and housing burden across California counties.
Using environmental risk measures from CalEnviroScreen and socioeconomic indicators, a machine learning pipeline was developed to identify the factors most associated with housing burden.

## Research Question
How do environmental pollution indicators relate to housing burden in California communities?

## Dataset
- CalEnviroScreen 3.0 Environmental Indicators
- California Median Household Income Data

## Methods

### Data Preprocessing
- Feature selection
- Missing value imputation
- County-level aggregation
- Data cleaning

### Exploratory Data Analysis
- Correlation heatmaps
- Pairwise relationship analysis

### Machine Learning
- Random Forest Regression
- Train-test split (80/20)

### Evaluation Metrics
- MAE
- RMSE
- R² Score

## Results

Key findings:
- Pollution Burden was among the strongest predictors.
- Environmental indicators showed varying levels of association with housing burden.
- Random Forest feature importance identified the most influential environmental variables.

## Tools Used

Python
Pandas
NumPy
Scikit-Learn
Matplotlib
Seaborn

## Authors

Chenfei, Shirley, Caleb, Yuna
