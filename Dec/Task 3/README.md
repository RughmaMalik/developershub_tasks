# Energy Consumption Time Series Forecasting

## Objective
This project focuses on forecasting hourly energy consumption using historical data. Accurate energy demand forecasting is crucial for utility companies to optimize power generation and reduce waste. This analysis utilizes time-series feature engineering and the XGBoost algorithm to predict future demand.
## Dataset
- Source: Kaggle – Household Power Consumption
- Attributes:
  - date, time
  - global_active_power, global_reactive_power, voltage, global_intensity
  - sub_metering_1, sub_metering_2, sub_metering_3
- Link: [Kaggle Dataset](https://www.kaggle.com/datasets/imtkaggleteam/household-power-consumption)

## Steps Performed
1.  **Preprocessing:** Parsed dates, handled missing values, and resampled data to an Hourly frequency to reduce noise.
2.  **Feature Engineering:** Created time-based features (Hour, Day of Week) and Lag features (Previous hour, Previous day).
3.  **Model Comparison:**
    * **ARIMA:** Good baseline, but struggled with complex multi-seasonal patterns.
    * **Prophet:** Excellent at capturing daily seasonality automatically.
    * **XGBoost:** Performed best when provided with specific lag features.

## Results (RMSE)
* **ARIMA:** 0.75
* **Prophet:** 0.62
* **XGBoost:** 0.50 (Best Performance)

*Conclusion:* The XGBoost model outperformed others because the energy consumption patterns are highly dependent on immediate past values, which the lag features captured effectively.

## How to Run
1. Open the notebook in Google Colab.
2. Upload the dataset (`household_power_consumption.csv`)
3. Run all cells to reproduce results.
