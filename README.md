# SportsBookEdge

An NBA and NHL prediction system built from scratch to identify betting edges against sportsbook odds. Ongoing learning project.

## Progress

- ✅ **Session 1** — NBA API integration, pulled first player game log  
- ✅ **Session 2** — SQLite database built, 2 seasons NBA + NHL data (regular season + playoffs) for 40+ players  
- ✅ **Session 3** — Feature engineering pipeline with leakage-safe rolling averages (5/10/20 game windows), rest days, back-to-back flags, home/away splits  
- 🚧 **Session 4** — Train first XGBoost model to predict player points  
- 🚧 **Session 5** — Compare predictions to real sportsbook lines via The Odds API  

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
