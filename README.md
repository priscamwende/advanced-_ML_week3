# advanced_ML_week3


### Air Quality Forecasting using Time Series Machine Learning Models
 
 ### **Project Overview**

This project focuses on building time series machine learning models to forecast air quality levels using historical atmospheric data. The dataset contains hourly measurements from multiple cities in Beijing, covering the period from March 2013 to February 2017.

The main objective is to predict pollutant concentrations such as PM2.5, PM10, SO2, NO2, CO, and O3, using both historical trends and meteorological factors.

 ##### **Objectives**
1. Analyze and preprocess multivariate time series air quality data
2. Engineer meaningful temporal and lag-based features
3. Build and compare multiple forecasting models
4. Evaluate model performance using error metrics
5. Visualize predictions vs actual pollution levels
6. Interpret pollution patterns and seasonality effects

#### Dataset Description

The dataset includes:
**Target Variables**
* PM2.5
* PM10
* SO2
* NO2
* CO
* O3

### **Feature Variables**
* Temperature
* Pressure
* Dew Point
* Rainfall
* Wind Speed
* Wind Direction
* Time Coverage
* Hourly data from 2013–03–01 to 2017–02–28

  #### **Project Workflow**
1. **Data Preprocessing**

Handling missing values (forward fill / interpolation)

Removing or treating outliers

Converting datetime columns

Ensuring consistent hourly time series format


2. **Feature Engineering**

Lag features (e.g., PM2.5(t-1), PM2.5(t-24))

Rolling statistics (mean, std, moving averages)

**Time-based features:**

Hour of day

Day of week

Month / seasonality

**Meteorological influence variables:**

Temperature

Wind speed

Pressure

3. **Model Selection & Training**

The following models were explored:

1. ARIMA (baseline univariate model)
2. SARIMA (seasonal time series modeling)
3. Advanced enhancement: Log-transformed rolling ARIMA


Each model was trained on the training set and tuned where applicable.

4.** Model Evaluation**

Models were evaluated using:

1. MAE 
2. RMSE
3. R² Score
4. AIC
5. BIC

Performance comparison was done to determine the best forecasting approach.

5. **Visualization**

Actual vs Predicted time series plots

Residual error analysis

Seasonal trend visualization

Pollution spike detection over time
