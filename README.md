# Bike Sharing Analysis

This project analyzes and predicts urban bike-sharing demand using environmental and temporal data. The goal is to identify usage patterns and build high-accuracy forecasting models to optimize bike availability in smart cities.

## Tech Stack
- Language: Python
- Libraries:   
  - Pandas, NumPy, Scikit-Learn, XGBoost, SHAP (for Data Processing & Modeling)    
  - Matplotlib, Seaborn (for Visualization)
 
## Technical Workflow
1. Data Processing & EDA
    - Aggregated and cleaned hourly (17,379 records) and daily (731 records) datasets.
    - Performed multi-variate correlation analysis to identify relationships between humidity, wind speed, and total rentals.
    - Visualized seasonal and monthly trends to capture long-term growth (2011 vs. 2012).

2. Machine Learning Modeling
    - Algorithms: Compared XGBoost Regressor and Support Vector Regression (SVR).
    - Optimization: Utilized GridSearchCV for hyperparameter tuning (Learning Rate, Max Depth, C, Epsilon).

    Performance: Achieved an $R^2$ Score of 0.99 through feature scaling and model optimization.

3. Model Interpretability (XAI)

    Implemented SHAP (SHapley Additive exPlanations) to break down the "black box" of the XGBoost model.

    Quantified the impact of features like temperature and working_day on final predictions.





## Features
- Exploratory Data Analysis (EDA) of bike-sharing datasets
- Data visualizations showing trends by time, location, and user type
- Insights into peak usage hours, seasonal patterns, and user behavior
- Optional predictive modeling for bike demand (if included in your project)

## Project Overview
The goal of this project is to explore bike rental data, identify key trends, and compare different machine learning models to predict demand.

## Methodology 

## Dataset
- Source: [Kaggle - Bike Sharing Dataset](https://www.kaggle.com/datasets/marklvl/bike-sharing-dataset)  
- Data is clean and well-structured, suitable for analysis and prediction tasks
- Includes: hourly and daily records with features such as weather, seasonality, and time  

Exploratory Data Analysis (EDA)
Analyzed the relationship between demand and variables like time, weather, and day of the week
Visualized seasonal and hourly patterns
Feature Engineering
Created new features like "hour_of_day", "day_of_week" based on timestamp data
Model Building
Built multiple predictive models including XGBoost and SVR
Compared models based on MAE, MSE, RMSE, and R² scores
Model Evaluation
Evaluated the performance of the models and selected the best one for demand prediction

## Key Tasks
- Performed Exploratory Data Analysis (EDA)
- Identified seasonal and hourly demand patterns
- Visualized trends using data visualization techniques
- Built and compared multiple predictive models

## Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib / Seaborn
- Scikit-learn

- 

## Results
- Discovered key factors affecting bike demand (e.g., time, weather, season)
- Evaluated model performance and selected the best-performing approach
