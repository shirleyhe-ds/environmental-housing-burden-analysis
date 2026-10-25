# Environmental Housing Burden Analysis
Analyzing the relationship between environmental pollution indicators and housing burden across California counties using exploratory data analysis and machine learning.

## Overview
This collaborative project explores the relationship between environmental conditions and housing burden in California. Using environmental data from CalEnviroScreen 3.0, we examine patterns among pollution indicators and housing burden, then use a Random Forest regression model to investigate which environmental features contribute most to housing-burden predictions.

## Research Question
How are environmental pollution indicators associated with housing burden across California communities, and which indicators are most important for predicting housing burden?

## Dataset
The project uses two datasets:
- CalEnviroScreen 3.0 Environmental Indicators: Environmental indicators, including ozone, PM2.5, diesel particulate matter, drinking water, pesticides, toxic releases, traffic, cleanup sites, groundwater threats, hazardous waste, solid waste, and pollution burden.
- California Median Household Income Data: A supplementary dataset used in the original project workflow.
The analysis selects environmental indicators and housing burden, removes rows with missing housing-burden values, and fills missing environmental predictor values using county-specific medians.

## Methods

### Data Preprocessing
- Selected relevant environmental indicators and housing burden.
- Removed observations with missing housing-burden values.
- Imputed missing environmental predictor values using county-specific medians.
- Removed the county-name column before modeling.

### Exploratory Data Analysis
- Created a correlation heatmap to examine relationships among variables.
- Used pair plots to explore relationships between individual environmental indicators and housing burden.

### Machine Learning
- Random Forest Regression
- Train-test split (80/20)

### Evaluation Metrics
- MAE
- MSE
- RMSE
- R² Score

## Visualizations

### Correlation Heatmap

<img src="images/correlation_heatmap.png" alt="Correlation heatmap of environmental indicators and housing burden" width="500">

### Environmental Indicators vs. Housing Burden

<img src="images/pairplot.png" alt="Pair plots comparing environmental indicators with housing burden" width="650">

### Random Forest Feature Importance

<img src="images/feature_importance.png" alt="Random Forest feature importance for housing-burden prediction" width="500">

## Results

The notebook calculates MAE (5.33), MSE (45.21), RMSE (6.72), and R^2 (0.38) on the test set. It also displays the five features with the highest Random Forest importance scores.

Key findings:
- Pollution Burden was among the strongest predictors.
- Environmental indicators showed varying levels of association with housing burden.
- Random Forest feature importance identified the most influential environmental variables.

## Tools Used

- Python
- Pandas
- NumPy
- Scikit-Learn
- Matplotlib
- Seaborn
