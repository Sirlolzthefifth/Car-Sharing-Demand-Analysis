# Car-Sharing Demand Analysis and Forecasting

## Overview

This project analyses hourly customer demand for a car-sharing service to identify patterns in usage and investigate how weather and seasonal conditions influence demand.

Using Python, the project applies data cleaning, exploratory data analysis, statistical testing and machine learning techniques to understand demand behaviour and evaluate forecasting approaches.

The analysis was completed as part of the **Databases and Data Analytics** module at Keele University.

## Objectives

- Explore hourly car-sharing demand and identify temporal patterns.
- Investigate the relationship between demand and weather-related variables.
- Apply statistical tests to identify factors associated with changes in demand.
- Develop and compare machine learning models for demand forecasting.
- Explore patterns in weather conditions using clustering techniques.

## Dataset

The dataset contains hourly observations of car-sharing activity, including:

- Date, hour and seasonal information
- Temperature and feels-like temperature
- Humidity and wind speed
- Weather conditions
- Customer demand

The dataset is included in this repository for reproducibility. Please refer to its original source and applicable usage terms before redistributing it.

## Methodology

### 1. Data Preparation
- Loaded and explored the dataset using Pandas and NumPy.
- Identified and removed duplicate records.
- Handled missing values through imputation.
- Prepared variables for statistical analysis and modelling.

### 2. Exploratory and Statistical Analysis
- Examined hourly and seasonal demand patterns.
- Used time-series visualisations to investigate demand and weather trends.
- Applied ANOVA and Pearson correlation to investigate relationships between demand and explanatory variables.
- Examined the statistical significance of weather, temperature, season and other factors.

### 3. Demand Forecasting
Implemented and evaluated the following forecasting approaches:

- ARIMA
- Random Forest Regressor
- Deep Neural Network (DNN)

Models were evaluated using Mean Squared Error (MSE).

### 4. Clustering
Applied K-Means and Agglomerative Clustering to explore groupings in weather-related observations and identify underlying patterns.

## Results

Key findings from the analysis include:

- Weather conditions, temperature, humidity, wind speed and season showed statistically significant relationships with demand in the reported analysis.
- ARIMA achieved an MSE of **0.2377** on the reported evaluation set.
- The Deep Neural Network achieved an MSE of **1.653**, compared with **1.955** for the Random Forest Regressor.
- K-Means and Agglomerative Clustering were explored to identify groups in the weather data.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Statistical analysis
- ARIMA
- Scikit-learn
- Deep Learning

## Repository Structure

```text
Car-Sharing-Demand-Analysis/
│
├── README.md
├── car_sharing_analysis.py
└── Dataset.csv
```

## Running the Project

1. Clone the repository:

   ```bash
   git clone https://github.com/YOUR_USERNAME/Car-Sharing-Demand-Analysis.git
   ```

2. Navigate into the project directory:

   ```bash
   cd Car-Sharing-Demand-Analysis
   ```

3. Install the required Python libraries. Check the imports in the Python script for the exact dependencies.

4. Run the analysis:

   ```bash
   python car_sharing_analysis.py
   ```
