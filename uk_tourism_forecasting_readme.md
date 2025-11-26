UK Tourism Forecasting Using Facebook Prophet

This project forecasts yearly tourist arrivals in the United Kingdom using the World Bank's international tourism dataset (via Kaggle). The goal is to build a complete time series forecasting pipeline using Facebook Prophet, including data cleaning, preparation, model development, and visualization.

Project Summary

Loaded and filtered the dataset to extract UK-specific tourism data.

Cleaned the dataset by removing non-year columns and missing values.

Converted the data from wide to long format for time series modeling.

Prepared Prophet-compatible fields (ds for dates, y for arrival values).

Built and trained a Prophet model to learn trends and seasonality patterns.

Forecasted future tourist arrivals for a 10-year period.

Created visualizations to show historical data, forecast trends, and seasonal behavior.

Technologies Used

Python

Pandas

Prophet

Matplotlib

Jupyter Notebook / VS Code Notebook

How to Run

Install dependencies:

pip install pandas prophet matplotlib


Open and run all cells in forecast.ipynb.

Files Included

forecast.ipynb – model training and forecasting

tourism.csv – input dataset

uk_tourism_forecast.csv – forecasted results

forecast_plot.png – forecast visualization

forecast_components.png – trend and seasonality plots
