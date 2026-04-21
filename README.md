# Predictive Paradox
## Electricity Demand Forecasting

## Results
- LightGBM MAPE: 5.57%
- Random Forest MAPE: 5.75%
- Linear Regression MAPE: 6.96%
- Best Model: LightGBM

## Dataset Used
- PGCB_date_power_demand.xlsx
- weather_data.xlsx
- economic_full_1.csv

## Approach
- Cleaned demand spikes using rolling z-score method
- Merged weather and economic data by datetime and year
- Engineered lag features (1h, 2h, 24h, 168h)
- Engineered rolling features (mean, std)
- Used chronological train/test split
- Compared 3 models: LightGBM, Random Forest, Linear Regression
