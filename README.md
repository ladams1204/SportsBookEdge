# SportsBookEdge

An NBA and NHL prediction system built from scratch to identify betting edges against sportsbook odds. Ongoing learning project.

## Progress

- ✅ **Session 1** — NBA API integration, pulled first player game log  
- ✅ **Session 2** — SQLite database built, 2 seasons NBA + NHL data (regular season + playoffs) for 40+ players  
- ✅ **Session 3** — Feature engineering pipeline with leakage-safe rolling averages (5/10/20 game windows), rest days, back-to-back flags, home/away splits  
- ✅ **Session 4** — First XGBoost model trained. Test RMSE 8.81 vs baseline 9.11 (small edge). SHAP analysis identified opponent-based features as the key gap.  
- 🚧 **Session 5** — Add opponent defensive rating, pace, teammate availability. Retrain. Target test R² > 0.20.  
- 🚧 **Session 6** — Integrate The Odds API. Compare model predictions to sportsbook lines to find edges.
## Stack

- Python (pandas, numpy, scikit-learn, xgboost)
- SQLite for local data persistence
- Google Colab as the dev environment
- Data sources: NBA Stats API, NHL Stats API, The Odds API

## Notebooks

| File | Purpose |
|------|---------|
| `01_data_exploration.ipynb` | Initial API testing |
| `02_build_database.ipynb` | Full ETL pipeline (NBA + NHL, regular season + playoffs) |
| `03_features.ipynb` | Feature engineering with anti-leakage rolling averages |
