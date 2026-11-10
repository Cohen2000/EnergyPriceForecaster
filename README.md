# Energy Price Forecaster

A machine-learning project for forecasting hourly German electricity prices over a 24-hour horizon. It combines SMARD electricity-market data with regional weather data and explores performance during the volatile year 2022.

## What it demonstrates

- Cleaning and aligning time-series data from several sources.
- Engineering lagged prices, rolling statistics, calendar features and regional weather features.
- Training 24 random-forest regressors, one per forecast horizon, in a daily backtest.
- Evaluating errors with MAE/RMSE and examining feature importance and price spikes.

## Start here

Open [Final.ipynb](Final.ipynb) for the complete workflow, saved outputs and discussion. The [price overview](price_plot_final.png) and [feature-importance plot](Feature_importance.png) give a quick visual introduction.

**Stack:** Python, pandas, NumPy, scikit-learn, Matplotlib and Jupyter.

## Reproducing the experiment

The notebook expects external market and weather files named in its data-loading section; those input files are not included in this repository. Install the packages listed in the notebook imports and supply the matching inputs before running it. Saved outputs can be read without rerunning training.

This is a research/coursework prototype. Historical backtest results are not evidence of live trading performance; availability of each feature and training target at the forecast origin must be checked before operational use.
