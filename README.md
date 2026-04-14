
## Forecasting Norway's GDP per Capita  
### A Time Series Approach

## Overview
This project focuses on forecasting Norway's GDP per capita using time series techniques. The analysis uses historical data from 1960 to 2024 and applies multiple forecasting models to evaluate their performance and predictive accuracy.

## Background
Norway is one of the wealthiest countries in the world, with its economy driven largely by oil and natural gas production, strong institutions, and a sovereign wealth fund. The GDP per capita series shows a strong upward trend with short-term shocks and minimal seasonality.

## Dataset
- Source: World Bank  
- Time Period: 1960 – 2024  
- Frequency: Annual  
- Variable: GDP per capita (constant USD)

### Train-Test Split
- Training Data: 1960 – 2015  
- Testing Data: 2016 – 2024  

## Methodology

### Data Preprocessing
- Cleaning and structuring the dataset  
- Time series visualization  
- Train-test split  

### Transformation
- Box-Cox Transformation (variance stabilization)  
- Differencing (stationarity)  
- ACF/PACF analysis  

## Models Used

### Baseline Models
- Mean Method  
- Naive Method  
- Drift Method  

### Advanced Models
- Exponential Smoothing (ETS)  
- ARIMA  

## Evaluation Metrics
- MAE (Mean Absolute Error)  
- RMSE (Root Mean Squared Error)  
- MAPE (Mean Absolute Percentage Error)  

## Results

| Model  | MAE     | RMSE    | MAPE (%) |
|--------|--------|--------|----------|
| Mean   | 28259  | 28308  | 36.54    |
| Naive  | 2469   | 2979   | 3.15     |
| Drift  | 2585   | 2947   | 3.33     |
| ETS    | 1255   | 1565   | 1.6      |
| ARIMA  | 610    | 896    | 0.8      |

## Key Insight
ARIMA performs the best with the lowest forecast errors, capturing both trend and underlying structure effectively.

## Key Findings
- Series is non-stationary and trend-dominated  
- Minimal seasonality  
- ARIMA captures dynamics best  
- Residual diagnostics confirm good model fit  

## Forecast (2025–2034)

| Year | Forecast (USD) |
|------|---------------|
| 2025 | 80194 |
| 2026 | 80713 |
| 2027 | 81224 |
| 2028 | 81729 |
| 2029 | 82228 |
| 2030 | 82719 |
| 2031 | 83204 |
| 2032 | 83682 |
| 2033 | 84153 |
| 2034 | 84618 |

## Conclusion
The study shows that model selection based on data characteristics is crucial. ARIMA emerges as the most suitable model for forecasting Norway’s GDP per capita, providing accurate and reliable predictions aligned with historical trends.
