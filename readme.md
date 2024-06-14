# Precipitation forecast

This project focuses on training machine learning models to predict precipitation values in Pacific Northwest. 

## Dataset

The dataset is "50" km resolution daily precipitation for the Pacific Northwest, 1949-94
provided by Martin Widmann and Christopher Bretherton of the University of Washington : http://research.jisao.washington.edu/data_sets/widmann/

![Dataset](image.png)

## Data Preprocessing

![Data Preprocessing workflow](image-4.png)

272 locations with 17 latitude and 16 longitude into 3 clusters with k means clustering

![clustered](image-1.png)

![Average Precipitation](image-2.png)

![Derived Temporal Features from time](image-3.png)

## Model Training 

3 Time Series models and 3 Non-Time Series models were trained to forecast precipitation

Time Series Models:
1. ARIMA
2. SARIMA
3. Exponential Smoothing (Holt Winter)

Non-Time Series Models:
1. Linear Regression
2. Random Forest
3. XGBoost

![Model Training Workflow](image-5.png)


## Ensemble Modeling 
![Reference](https://www.analyticsvidhya.com/blog/2018/06/comprehensive-guide-for-ensemble-models/)

Best Performance models are ensemble via weighted average (0.5 each model) and model stacking with Linear Regression. 

![weighted average](image-6.png)

![model stacking](image-7.png)





