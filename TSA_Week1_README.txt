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
   - runs in Colab, VS Code, Kaggle, GitHub Classroom, anywhere
   - NO file upload and NO setup: all three CSVs are stored compressed
     inside the notebook, so the data can never go missing
   - pick a CSV by editing `filename` in the cell under "1. Choose a dataset"
   - inspect
   - parse/sort time
   - time plot
   - chronological train/test split
   - naive forecast baseline
   - MAE/RMSE
   - optional lag-1 plot
   - VS Code: use the project .venv Python 3 kernel (already registered)

All three datasets are synthetic teaching data.

How to open the notebook on Google Colab
- go to https://colab.research.google.com
- File > Upload Notebook... and choose
  TSA_Week1_Time_Series_Baseline_VSCode.ipynb
  (dragging the .ipynb onto the Colab page works too)
- Runtime > Run all
- nothing else: the notebook carries its own copy of the data

How to run it in VS Code
- open the folder, then the notebook
- pick the Python 3 kernel (the project .venv)
- Runtime > Run All

About the "Choose file" button
The Colab file picker only works inside the Colab website. VS Code cannot
draw that dialog, so the notebook checks where it is running and skips the
picker when it is not on the Colab page; the built-in copy of the CSV is used
instead. Every environment therefore gives the same numbers:
MAE 244.17, RMSE 271.58 (monthly sales dataset).

If the CSVs are ever hosted somewhere public, put that raw URL in RAW_BASE and
the notebook downloads the CSV instead of using the built-in copy.
