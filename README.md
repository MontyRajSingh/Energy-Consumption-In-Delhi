
 Energy Consumption Forecasting in Delhi Using Machine Learning

This project focuses on forecasting hourly electricity demand for the city of Delhi, India using machine learning techniques. The objective is to support smart grid planning, demand management, and energy optimization by predicting future energy consumption based on historical usage, weather conditions, and solar power generation.

⸻

Problem Statement

Electricity demand fluctuates throughout the day due to factors like temperature, solar energy availability, working hours, weekends, and holidays. Accurate forecasting is crucial for:
	•	Efficient power grid operation
	•	Reducing generation cost
	•	Preventing blackouts / overload
	•	Renewable energy integration
	•	Smart city energy planning

This project builds an ML model to accurately forecast energy demand using real-world data from Delhi, India.



 Project Objectives
	•	Perform exploratory data analysis (EDA) on Delhi electricity consumption
	•	Engineer time-series features (lags, rolling windows, weekdays, weather)
	•	Train and compare models:
	•	Linear Regression
	•	Random Forest
	•	XGBoost (Best Performance)
	•	Evaluate model using MAE and RMSE
	•	Visualize actual vs predicted demand
	•	Demonstrate future load prediction capabilities

⸻

 Techniques Used

Category                Methods

Data Preprocessing      Time parsing, handling missing values, sorting, indexing
Feature Engineering     Lag features, rolling mean, weekday/weekend, holiday, hour-of-day
Models                  Linear Regression, Random Forest, XGBoost
Evaluation Metrics      MAE, RMSE
Visualization           Load curves, error histogram, feature importance

📊 Dataset Description
Hourly dataset for Delhi (8,737 rows — full year) containing:
Feature             Description

timestamp           Date + hour
day_of_week         0–6
hour_of_day         0–23
is_weekend          1/0
temperature         °C
is_holiday          1/0
solar_generation    MW
load (Target)       Electricity demand in MW

  Model Performance
Model                    MAE ↓           RMSE ↓

Linear Regression      ~416.23          ~533.92
Random Forest          ~220.88          ~289.97
XGBoost                ~193.56          ~255.12
✅ XGBoost gave the best forecasting accuracy



 Key Visualizations
	•	Actual vs Predicted Demand
	•	Zoomed prediction (first 200 hours)
	•	Error distribution plot
	•	Residuals vs time
	•	Feature importance plot

Temperature, hour-of-day, previous load values, and solar generation are most important for forecasting.


