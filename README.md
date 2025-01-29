# Project Name
> Prediction of Demand for Shared Bikes


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Regression Analysis](#regression-analysis)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)


## General Information
- This project involves building a multiple linear regression model to predict the demand for shared bikes.
- **Business Problem:** BoomBikes, a US-based bike-sharing service, has experienced revenue drops during the COVID-19 pandemic. To prepare for post-pandemic demand, the company wants to identify factors affecting bike demand and use them to strategize effectively.
- **Dataset Used:** The dataset contains daily bike demand data with variables such as weather conditions, seasonal effects, and temporal factors (e.g., year, month).
- The goal is to analyze how different variables influence bike demand (`cnt`) and create a predictive model to guide business decisions.


## Regression Analysis
### Problem Statement:
- A bike-sharing system allows short-term bike rentals, often through computer-controlled docks. BoomBikes aims to understand the factors driving demand for its services in the American market post-quarantine.

### Key Objectives:
1. Identify significant variables affecting demand.
2. Understand how well these variables explain the variations in demand.

### Summary of OLS Regression Results:
- **Dependent Variable:** Total demand (`cnt`)
- **Adjusted R-squared:** 0.823 (Model explains 82.3% of the variance in bike demand)
- **Significant Predictors:**
  - Positive Effects: `yr`, `temp`, `summer`, `winter`
  - Negative Effects: `hum`, `windspeed`, `Light Snow`, `Mist`, `Monday`, `Sunday`
- **Residual Diagnostics:**
  - Durbin-Watson: 2.011 (No significant autocorrelation)
  - Omnibus: Residuals show some deviation from normality.
- **VIF Analysis:** No multicollinearity issues (all VIFs < 5).

### Recommendations:
- Retain all predictors as they are statistically significant and show minimal multicollinearity.
- Further refine the model through residual analysis and cross-validation.


## Technologies Used
- Python 3.8+
- Pandas
- NumPy
- Statsmodels
- Matplotlib
- Scikit-learn


## Conclusions
- The model successfully identifies significant predictors of bike demand and explains 82.3% of the variance.
- Meteorological variables (`temp`, `hum`, `windspeed`, `weather conditions`) and temporal factors (`yr`, `season`) significantly influence demand.
- Insights can help BoomBikes adjust pricing strategies, marketing campaigns, and operational planning to optimize revenue.


## Acknowledgements
- This project was inspired by the Linear Regression assignment from the IIIT Bangalore program.
- Dataset provided by BoomBikes.
- References: Statsmodels documentation, Scikit-learn tutorials.


## Contact
Created by [Reetesh Nigam] - feel free to contact me for any questions or collaboration opportunities.

