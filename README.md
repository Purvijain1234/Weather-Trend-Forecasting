# 🌦️ Weather Trend Forecasting

> **PM Accelerator Technical Assessment**

This project analyzes the **Global Weather Repository** dataset to explore global weather trends and build a basic forecasting model using Machine Learning and Time Series Analysis. The project demonstrates an end-to-end data science workflow, including data preprocessing, exploratory data analysis, feature engineering, forecasting, and model evaluation.

---

# PM Accelerator Mission

PM Accelerator empowers aspiring professionals through real-world projects, hands-on learning, and industry-focused mentorship in Artificial Intelligence, Data Science, Product Management, and Software Engineering. The goal is to bridge the gap between academic learning and practical implementation.

---

# Project Objectives

The primary objectives of this project are to:

- Clean and preprocess weather data
- Handle missing values and duplicate records
- Perform Exploratory Data Analysis (EDA)
- Analyze weather trends and correlations
- Generate visualizations for temperature and precipitation
- Use the **last_updated** feature for time series analysis
- Build a basic weather forecasting model
- Evaluate model performance using regression metrics
- Perform additional environmental and geographical analyses

---

# Dataset

**Dataset Name:** Global Weather Repository

**Source:** https://www.kaggle.com/datasets/nelgiriyewithana/global-weather-repository

The dataset contains over **109,000** weather observations collected from cities around the world and includes more than **40 weather-related features**, such as:

- Temperature
- Humidity
- Wind Speed
- Atmospheric Pressure
- Precipitation
- Visibility
- UV Index
- Cloud Cover
- Air Quality
- Sunrise & Sunset Information

---

# Repository Structure

```
Weather-Trend-Forecasting/
│
├── dataset/
│   ├── GlobalWeatherRepository.csv
│   └── cleaned_datasets.csv
│
├── notebooks/
│   ├── Data_Cleaning.ipynb
│   ├── EDA.ipynb
│   └── Model.ipynb
│
├── README.md
├── REPORT.md
├── requirements.txt
├── LICENSE
└── .gitignore
```

---

# Workflow

## 1. Data Cleaning & Preprocessing

- Loaded the dataset
- Inspected data types
- Handled missing values
- Removed duplicate records
- Converted `last_updated` into datetime format
- Created time-based features
- Performed outlier analysis

---

## 2. Exploratory Data Analysis

EDA was conducted to understand weather patterns through various visualizations and statistical analyses.

Analysis included:

- Temperature Distribution
- Humidity Distribution
- Wind Speed Distribution
- Precipitation Distribution
- Correlation Heatmap
- Monthly Temperature Trends
- Country-wise Weather Analysis
- Outlier Detection

---

## 3. Time Series Feature Engineering

The `last_updated` column was converted into datetime format and used to generate:

- Year
- Month
- Day
- Day of Week
- Day of Year

These features were used to train the forecasting model.

---

## 4. Model Building

A **Linear Regression** model was implemented to forecast temperature.

### Target Variable

- Temperature (°C)

### Features Used

- Year
- Month
- Day
- Day of Week
- Day of Year

---

## 5. Model Evaluation

The forecasting model was evaluated using:

- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- R² Score

These metrics were used to measure prediction accuracy and overall model performance.

---

# Additional Analyses

## Environmental Impact Analysis

Analyzed the relationship between weather parameters and air quality indicators including:

- PM2.5
- PM10
- Carbon Monoxide
- Ozone

This analysis highlights how atmospheric conditions influence environmental quality.

---

## Geographical Pattern Analysis

Compared weather conditions across different countries to identify:

- Temperature variations
- Rainfall patterns
- Regional climatic differences

This provides a broader understanding of global weather diversity.

---

# Key Insights

- The dataset contains over **109,000** global weather observations with more than **40 weather-related features**.
- Duplicate records were removed and missing values were handled during preprocessing.
- Extreme temperature and precipitation values were retained because they represent genuine weather events rather than data errors.
- Most temperatures fall between **17°C and 28°C**, with an average temperature of approximately **22.4°C**.
- Wind speed values are generally moderate, while precipitation is highly right-skewed due to many days with no rainfall.
- Correlation analysis revealed meaningful relationships among weather variables and air quality indicators.
- Time-based features extracted from **last_updated** improved the forecasting process.
- Linear Regression served as a reliable baseline model for weather trend forecasting.

---

# Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

---

# Installation

Clone the repository

```bash
git clone https://github.com/Purvijain1234/Weather-Trend-Forecasting.git
```

Navigate to the project directory

```bash
cd Weather-Trend-Forecasting
```

Install the required dependencies

```bash
pip install -r requirements.txt
```

---

# How to Run

Execute the notebooks in the following order:

1. **01_Data_Cleaning.ipynb**
2. **02_EDA.ipynb**
3. **03_Model_Building.ipynb**

---

# Results

The project successfully demonstrates:

- Data Cleaning & Preprocessing
- Exploratory Data Analysis
- Time Series Feature Engineering
- Weather Forecasting using Machine Learning
- Model Evaluation
- Environmental Impact Analysis
- Geographical Pattern Analysis

---

# Future Improvements

Possible enhancements include:

- ARIMA-based forecasting
- Prophet time series forecasting
- Random Forest and XGBoost comparison
- Interactive Streamlit dashboard
- Seasonal climate analysis
- Model deployment

---

# Author

**Purvi Jain**
GitHub: https://github.com/Purvijain1234

---

## ⭐ If you found this project useful, consider giving the repository a star.
