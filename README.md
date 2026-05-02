# Bike Sharing Analysis

This project analyzes and predicts urban bike-sharing demand using environmental and temporal data. The goal is to identify usage patterns and build high-accuracy forecasting models to optimize bike availability in smart cities.

## Dataset
- Source: [Kaggle - Bike Sharing Dataset](https://www.kaggle.com/datasets/marklvl/bike-sharing-dataset)  
- Data is clean and well-structured, suitable for analysis and prediction tasks
- Includes: hourly and daily records with features such as weather, seasonality, and time  

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
    - Performance: Achieved an $R^2$ Score of 0.99 through feature scaling and model optimization.

3. Model Interpretability (XAI)  
    - Implemented SHAP (SHapley Additive exPlanations) to break down the "black box" of the XGBoost model.
    - Quantified the impact of features like temperature and working_day on final predictions.

## Results & Visuals
- Bike-sharing usage grows over time but is highly influenced by weather, weekdays, and special events.
- Predictive models (SVR, XGBoost) can forecast demand accurately, helping cities and companies manage resources efficiently.
- Temperature and user type are the most important predictors of demand.
- Spatial analysis and real-time monitoring further optimize urban mobility.
