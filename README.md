# Sudan: Conflict & Socio-Economic Indicators (2000–2024)

This repository analyzes the relationship between political violence (events and fatalities) and macroeconomic indicators in Sudan.

## Data

- `data/sudan_merged_conflict_economy.csv`: Merged conflict–economy dataset (annual).
- `data/sudan_train.csv`: Training set for modeling.
- `data/sudan_test.csv`: Time-based test set.

## Notebook

- `sudan_conflict_economy.ipynb`: End-to-end workflow
  - Data loading and cleaning
  - Feature engineering (per-100k, rolling averages, lags)
  - Exploratory analysis (time series, correlations, regional patterns)
  - Modeling (baseline, Random Forest with time-series CV)
  - Diagnostics and interpretation (feature importance, residuals)

## Reproducibility

- Python: 3.x
- Core libraries: `pandas`, `numpy`, `scikit-learn`, `matplotlib`, `seaborn`, `plotly`
- Random seed: `RANDOM_SEED = 42`

## Next steps

- Add SHAP-based explainability
- Extend to sub-national (Admin1) modeling
- Increase temporal resolution (monthly/quarterly)

sudan-conflict-economy-2000-2024/
│
├─ data/
│   ├─ sudan_merged_conflict_economy.csv
│   ├─ sudan_train.csv
│   └─ sudan_test.csv
│
├─ notebooks/
│   └─ 01_sudan_conflict_economy.ipynb
│
├─ reports/
│   └─ sudan_conflict_economy_report.md 
│
├─ README.md
└─ requirements.txt  
