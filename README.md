# Fashion AI Adoption Signals (Public Data)

This project analyzes early adoption signals for AI-enabled fashion experiences (price intelligence and virtual try-on) using public behavioral proxies:
- Apple App Store review velocity (iTunes RSS customerreviews feed)
- Weekly aggregation of review counts and average ratings
- Short-horizon forecasting using Prophet (next 8 weeks)

## Outputs
- Adoption proxy leaderboard: total reviews by category
- Weekly review velocity tables by category/app
- Prophet forecasts with uncertainty intervals (yhat_lower, yhat_upper)

## How to run
1. Install Python packages:
   pip install -r requirements.txt
2. Run:
   python src/run_pipeline.py

## Notes
- Review volume is an engagement proxy (people who review), not total installs.
- Forecasts are directional and short-horizon due to sparse early-stage signals.
