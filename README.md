# Walmart Sales Forecasting & Time Series Analysis

## Overview
Can historical sales data accurately forecast short-term weekly sales? This project builds and compares three forecasting models using Walmart store data, with results focused on predictive performance rather than causal inference.

## Data Source & Size
- **Source:** Walmart Recruiting Store Sales Forecasting (Kaggle)
- **Records:** 421,570 weekly sales observations
- **Scope:** 45 stores, 81 departments
- **Period:** February 2010 – October 2012 (143 weeks)

## Key Findings
- Strong seasonality: December and Q4 consistently showed peak sales; holiday weeks produced a 7.1% average sales increase
- Top 5 stores drove 30% of total revenue; top store generated $301M over the period
- Prophet outperformed all models with 2.47% MAPE — a 42% improvement over the naive baseline
- 4-week-ahead forecasts showed rising sales into the holiday season, consistent with historical patterns

## Tools & Skills Demonstrated
- **Language:** Python (pandas, numpy, matplotlib, seaborn, prophet)
- **Techniques:** Exploratory data analysis, time series decomposition, train-test split, model evaluation (MAPE, MAE, RMSE), confidence interval forecasting
- **Outputs:** Forecast visualizations, model comparison charts, 4-week predictions with 95% confidence intervals
