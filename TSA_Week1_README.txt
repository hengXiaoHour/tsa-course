TSA Week 1 teaching pack

Files:
1. tsa_week1_synthetic_monthly_sales.csv
   - 60 monthly observations
   - target: sales_units
   - clear trend + seasonal pattern
   - recommended first dataset

2. tsa_week1_synthetic_daily_demand.csv
   - 180 daily observations
   - target: electricity_demand_kwh
   - includes temperature and weekend indicator
   - useful for discussing time order and predictor variables

3. tsa_week1_synthetic_weekly_rainfall.csv
   - 104 weekly observations
   - target: rainfall_mm
   - includes soil_moisture_pct
   - useful agriculture-flavoured example

4. TSA_Week1_Time_Series_Baseline_VSCode.ipynb
   - local VS Code version
   - pick a CSV by editing `filename` in cell 2
   - inspect
   - parse/sort time
   - time plot
   - chronological train/test split
   - naive forecast baseline
   - MAE/RMSE
   - optional lag-1 plot
   - use the project .venv Python 3 kernel (already registered)

All three datasets are synthetic teaching data.
