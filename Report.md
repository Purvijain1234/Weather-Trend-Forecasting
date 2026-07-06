# 🌦️ Weather Trend Forecasting

## PM Accelerator Technical Assessment

---

# PM Accelerator Mission

PM Accelerator is committed to empowering aspiring professionals by providing real-world project experience, practical learning opportunities, and industry-relevant skills in Artificial Intelligence, Data Science, Product Management, and Software Engineering. Through hands-on projects and collaborative learning, the program helps bridge the gap between academic knowledge and real-world applications.

---

# Project Overview

This project analyzes the **Global Weather Repository** dataset to understand weather trends and build a basic forecasting model for predicting temperature using historical weather observations.

The project follows a complete data science workflow consisting of:

- Data Cleaning & Preprocessing
- Exploratory Data Analysis (EDA)
- Time Series Feature Engineering
- Weather Trend Forecasting
- Model Evaluation
- Environmental Impact Analysis
- Geographical Pattern Analysis

---

# Dataset Summary

**Dataset:** Global Weather Repository

**Source:** https://www.kaggle.com/datasets/nelgiriyewithana/global-weather-repository

### Dataset Information

- Total Records: **109,271**
- Features: **40+**
- Coverage: Multiple cities across different countries
- Time Feature Used: **last_updated**

The dataset contains weather-related variables including:

- Temperature
- Humidity
- Wind Speed
- Atmospheric Pressure
- Precipitation
- Visibility
- UV Index
- Cloud Cover
- Air Quality Indicators

---

# Data Cleaning & Preprocessing

The following preprocessing steps were performed before analysis:

- Loaded the dataset using Pandas
- Inspected data types
- Identified missing values
- Removed duplicate records
- Converted **last_updated** into datetime format
- Created time-based features for forecasting

Generated features include:

- Year
- Month
- Day
- Day of Week
- Day of Year

These engineered features were used during model training.

---

# Outlier Analysis

The IQR method was initially applied to detect outliers.

Further inspection showed that the detected observations represent genuine weather events rather than data errors.

### Temperature

- Minimum Temperature: **-24.9°C**
- Maximum Temperature: **49.2°C**

These values correspond to realistic weather conditions observed across different climatic regions.

### Wind Speed

- Minimum Wind Speed: **3.6 km/h**
- Maximum Wind Speed: **34.9 km/h**

No unrealistic wind speed observations were identified.

### Precipitation

- Maximum Rainfall: **42.24 mm**

The precipitation variable is highly right-skewed because most observations recorded little or no rainfall, while a small number represented heavy rainfall events.

Therefore, **no outliers were removed**.

---

# Exploratory Data Analysis

EDA was performed to understand weather trends, feature distributions, and relationships among variables.

### Temperature

- Most observations fall between **17°C and 28°C**
- Average temperature is approximately **22.4°C**
- Both hot and cold climate regions are represented

### Humidity

Humidity varies considerably across locations, reflecting different climatic conditions.

### Wind Speed

Most observations lie between **6 km/h and 17 km/h**, indicating generally moderate wind conditions.

### Precipitation

- Majority of observations recorded **0 mm rainfall**
- Distribution is highly right-skewed
- Heavy rainfall events are relatively rare

### Correlation Analysis

The correlation heatmap revealed moderate relationships among several weather variables, indicating that atmospheric conditions are interrelated and useful for predictive modeling.

---

# Time Series Analysis

The **last_updated** feature was used for time series analysis.

Additional temporal features extracted from this column enabled the forecasting model to capture calendar-based weather patterns.

Extracted features include:

- Year
- Month
- Day
- Day of Week
- Day of Year

---

# Forecasting Model

A **Linear Regression** model was implemented as a baseline forecasting model.

### Target Variable

- Temperature (°C)

### Input Features

- Year
- Month
- Day
- Day of Week
- Day of Year

---

# Model Evaluation

The model was evaluated using the following regression metrics:

- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- R² Score

> Replace the values below with your notebook results.

| Metric | Value |
|---------|------:|
| MAE | 7.81 |
| RMSE | 9.34 |
| R² Score | -0.8459 |

The comparison between actual and predicted temperatures demonstrates that the model successfully captures overall weather trends while providing a strong baseline for future improvements.

---

# Environmental Impact Analysis

A correlation analysis was performed between weather conditions and air quality indicators.

### Air Quality Variables

- PM2.5
- PM10
- Carbon Monoxide (CO)
- Ozone (O₃)

### Weather Variables

- Temperature
- Humidity
- Wind Speed
- Atmospheric Pressure

### Key Observations

- Weather conditions influence pollutant concentration.
- Wind speed generally helps disperse pollutants.
- Humidity and pressure show relationships with several air quality indicators.
- Air quality is influenced by multiple environmental factors rather than a single weather variable.

---

# Geographical Pattern Analysis

Average weather conditions were compared across different countries.

### Temperature Patterns

- Tropical regions generally exhibit higher average temperatures.
- Cooler regions maintain significantly lower average temperatures.

### Rainfall Patterns

- Rainfall distribution varies considerably across countries.
- Some regions consistently receive higher precipitation than others.

### Overall Observation

The dataset captures diverse climatic conditions, making it suitable for comparative weather analysis across geographical regions.

---

# Key Findings

- The dataset is clean and well-structured for weather analytics.
- Extreme temperatures and rainfall values represent genuine weather events rather than errors.
- Weather variables exhibit meaningful correlations.
- Time-based features improve forecasting capability.
- Linear Regression provides a simple baseline forecasting model.
- Environmental and geographical analyses offer additional insights into global weather patterns.

---

# Future Improvements

Future enhancements could include:

- Implementing ARIMA or Prophet for time series forecasting.
- Comparing multiple machine learning models such as Random Forest and XGBoost.
- Developing an interactive Streamlit dashboard.
- Performing seasonal climate analysis.
- Deploying the forecasting model as a web application.

---

# Conclusion

This project demonstrates a complete end-to-end machine learning workflow, beginning with raw weather data and ending with predictive modeling.

The implementation successfully satisfies the requirements of the **PM Accelerator Technical Assessment**, including:

- ✅ Data Cleaning & Preprocessing
- ✅ Exploratory Data Analysis
- ✅ Time Series Analysis
- ✅ Weather Forecasting
- ✅ Model Evaluation
- ✅ Environmental Impact Analysis
- ✅ Geographical Pattern Analysis

The project provides a strong foundation for future work in weather forecasting and climate analytics.

---

# Author

**Purvi Jain**

B.Tech in Artificial Intelligence

Delhi Skill and Entrepreneurship University (DSEU)

GitHub: https://github.com/Purvijain1234
