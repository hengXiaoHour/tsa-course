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
   - runs in VS Code AND in Google Colab (same file, no edits needed)
   - pick a CSV by editing `filename` in cell 3
   - inspect
   - parse/sort time
   - time plot
   - chronological train/test split
   - naive forecast baseline
   - MAE/RMSE
   - optional lag-1 plot
   - VS Code: use the project .venv Python 3 kernel (already registered)
   - Colab: upload the notebook, then the first code cell opens a file
     picker for the CSV; pick it once and the whole run reuses it

All three datasets are synthetic teaching data.

How to open the notebook on Google Colab
- go to https://colab.research.google.com
- File > Upload Notebook... and choose
  TSA_Week1_Time_Series_Baseline_VSCode.ipynb
  (dragging the .ipynb onto the Colab page works too)
- Runtime > Run all
- when the first code cell asks for a file, choose
  tsa_week1_synthetic_monthly_sales.csv

If the CSVs are ever hosted somewhere public, put that raw URL in
RAW_BASE in cell 3 and the notebook downloads the CSV instead of asking.
