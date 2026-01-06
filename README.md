# Walmart-Sales-Forecasting-Time-Series-Analysis
This project examines the question: Can historical Walmart sales data be used to accurately forecast short-term weekly sales? The results focus on predictive performance rather than causal inference, as the analysis is observational and based solely on past sales patterns without external demand drivers such as pricing, promotions, or weather.

The analysis uses publicly available Walmart sales data covering 421,570 weekly observations across 45 stores and 81 departments from February 2010 to October 2012. Key findings show strong seasonal and holiday effects, with December and Q4 consistently exhibiting peak sales. Among the forecasting approaches tested, the Facebook Prophet model achieved the highest accuracy, with a 2.47% MAPE, representing a 42% improvement over a naive baseline.

Repository Contents

The repository contains all files necessary to replicate the analysis:

exploratory_analysis.ipynb – Data cleaning, exploratory analysis, and visualization

forecasting_models.ipynb – Model construction, evaluation, and forecasting

forecast_summary.json – Summary of model performance metrics

plots – All generated plots and figures

Walmart Sales Forecasting & Time Series Analysis.pdf – Presentation summarizing methodology and results

Data Source

All data come from the Walmart Recruiting Store Sales Forecasting dataset (Kaggle):
https://www.kaggle.com/competitions/walmart-recruiting-store-sales-forecasting

Reproducing the Analysis

To reproduce the results, the user only needs to:

Download the Walmart sales dataset from the Kaggle link above

Install required Python packages: pandas, numpy, matplotlib, seaborn, prophet

Update file paths in the notebooks if needed

Run exploratory_analysis.ipynb, then forecasting_models.ipynb

All data cleaning, aggregation, model training, evaluation (MAE, RMSE, MAPE), and visualization are automated within the notebooks.

Results

The analysis compares three forecasting approaches: a naive baseline, a 4-week moving average, and Facebook Prophet. Prophet performs best across all error metrics and produces 4-week-ahead forecasts with 95% confidence intervals, suitable for short-term inventory and staffing planning.

The figures folder contains time series plots, model comparison charts, forecast visualizations, and exploratory analyses of sales distributions, store performance, and holiday effects. The accompanying PDF presentation summarizes the empirical findings and discusses limitations and potential extensions.

Key Limitations

Forecasts are based only on historical sales, excluding external demand drivers

Results are aggregated across stores and departments

Long-term forecasts beyond the short horizon are not evaluated

Findings are predictive, not causal

This project is intended as an applied demonstration of time series forecasting and model evaluation in a retail context.
