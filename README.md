# Indigo Passenger Data Analysis

This repository contains a data analysis project on Indigo Airlines' passenger traffic. The project processes and analyzes passenger data from April 2014 to December 2024.

## Data Processing

- **Data Loading**: The dataset is loaded from a CSV file using pandas.
- **Preprocessing**:
  - The `MONTH` column is converted to a datetime format.
  - The `PASSENGERS` column is cleaned by removing commas and converting it to an integer type for accurate analysis.
- **Sorting**: The data is sorted by date for sequential analysis.

## Machine Learning Procedure

1. **Time Series Forecasting**:
   - A **SARIMA (Seasonal AutoRegressive Integrated Moving Average)** model was used to predict the future passenger traffic. SARIMA is well-suited for time series data with trends and seasonal patterns.
   - The model was trained using historical passenger data, capturing seasonality, trend, and any periodic patterns.

2. **COVID-19 Impact**:
   - A binary indicator, `COVID_EFFECT`, was introduced to account for the significant drop in passenger numbers from March 2020 to early 2021. This helped the model adjust predictions by considering the external impact of the pandemic.

3. **Model Evaluation**:
   - The model's performance was evaluated using standard metrics such as Mean Absolute Error (MAE) and Root Mean Squared Error (RMSE) to ensure the accuracy of the predictions.

## Results

The final analysis predicts the total number of passengers Indigo will carry by the end of 2024, accounting for seasonal fluctuations and the ongoing recovery from the COVID-19 pandemic.

---

**Note**: The numbers that Indigo is expected to reach by the end of the year are projected.  
Verify these numbers at the official website (https://www.dgca.gov.in/digigov-portal/?page=jsp/dgca/InventoryList/dataReports/aviationDataStatistics/airTransport/domestic/monthly/indigo24.pdf&main259/4184/servicename), which gets updated every month.
