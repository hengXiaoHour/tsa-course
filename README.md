# TSA Course — Time Series Analysis

Coursework notebooks for Time Series Analysis: baselines, lags, autocorrelation — with datasets embedded so every notebook runs anywhere (Colab, VS Code, Kaggle).

## Contents

- `TSA_Week1_Time_Series_Baseline_VSCode.ipynb` — trend + seasonality, train/test split, naive-forecast baseline (MAE/RMSE), lag-1 plot
- `data/phnom_penh_monthly_precipitation_2015_2025_long.csv` — Phnom Penh monthly precipitation 2015–2025 (132 obs, source table alongside)
- `tsa_week1_synthetic_*.csv` — 3 synthetic teaching datasets (monthly sales, daily demand, weekly rainfall)
- `figures/` — time plot, seasonal plot, seasonal subseries, unusual observations
- `TSA_Week1_README.txt` — original teaching-pack notes

## Run it

VS Code (recommended — project `.venv` + registered kernel):

```bash
python3 -m venv .venv
.venv/bin/pip install pandas numpy matplotlib jupyter
code TSA_Week1_Time_Series_Baseline_VSCode.ipynb
```

Or Colab: File → Upload Notebook → pick the `.ipynb` — no data upload needed, CSVs are embedded (gzip+base64) with local-file → download → picker → built-in fallback.

## Week 1 baseline

Naive forecast on synthetic monthly sales: **MAE 244.17 / RMSE 271.58**, 48 train / 12 test, 4 figures.
