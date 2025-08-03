# EUR/USD Price Regression (15-Minute Data, 2000–2020)

This project applies regression models to historical EUR/USD Forex data recorded at 15-minute intervals between 2000 and 2020.

## Dataset

**Filename:** `EURUSD-2000-2020-15m.csv`

**Columns:**
- `DATE_TIME`: Timestamp of the 15-minute interval (format: YYYY-MM-DD HH:MM)
- `HIGH`: Highest price within the interval
- `LOW`: Lowest price within the interval
- `OPEN`: Opening price of the interval
- `CLOSE`: Closing price of the interval

## Objective

To develop models that predict future prices or returns based on historical price patterns.

### Example Prediction Targets:
- Next `CLOSE` price (regression)
- Price change: `CLOSE(t+1) - CLOSE(t)`
- Log return: `log(CLOSE(t+1) / CLOSE(t))`

## Workflow Overview

1. **Data Preprocessing**
   - Convert `DATE_TIME` to datetime format
   - Set time as index (if needed)
   - Handle missing values and outliers
   - Feature engineering (e.g., lag features, rolling means)

2. **Exploratory Data Analysis**
   - Time series plots
   - Correlation analysis
   - Seasonality and trend checks

3. **Modeling**
   - Linear Regression
   - Ridge/Lasso Regression
   - Random Forest Regressor
   - XGBoost Regressor

4. **Evaluation**
   - Metrics: MAE, RMSE, R²
   - Visualization of predictions vs actual prices

## Future Work

- Include technical indicators (RSI, MACD, etc.)
- Try deep learning models (LSTM, GRU)
- Integrate walk-forward validation

## Authors

- Seyed Ali Rashidi
- Mahdi Miri
- Mohammad Aghaei Molasaraei


