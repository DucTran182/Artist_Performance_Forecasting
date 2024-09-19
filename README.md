# Artist_Performance_Forecasting

## Table of Contents
1. [Introduction](#introduction)
2. [Setup and Installation](#setup-and-installation)
3. [Run The Code](#run-the-code)
4. [Conclusion](#conclusion)

## Introduction
This project is to design a performance forecasting model for the singer "ISAAC," predicting his growth over the next five years (2024-2029) on platforms like YouTube and Spotify. The ISAAC performance forecasting model aims to predict the future trajectory of his music career, focusing on YouTube and Spotify metrics. The result will guide investment decisions for a company seeking to capitalize on ISAAC’s potential growth.

## Setup and Installation
To run the model locally, follow these steps:

1. Install python3.11.9.
2. Set up Jupyter Notebook development environment (pip install pandas, matplotlib, scikit-learn, statsmodels, prophet)
3. Clone this repository.
4. Download dataset

## Run the code
After installing everything, you just need to run the main.ipynb to get the forecasting results of ISAAC's performance on Spotify and YouTube. 
P/s: I have already converted the data from spreadsheet to CVS format.

To run, follow these 4 steps:
#### Step 1: Load data into the code  

#### Step 2: EDA to understand its structure and distribution as well as to prepare and transform for modeling     

#### Step 3: Visualize the data to get an overview before forecasting with matplotlib.pyplot  

#### Step 4: Build a forecasting model with Prophet  
##### Model Selection:  
We used Facebook Prophet, a robust time series forecasting model. Prophet is well-suited for capturing trends and seasonality in streaming data, making it ideal for predicting future performance.

##### Data Preparation:  
The dataset includes Spotify stream data from 2017 to September 2024, along with key metadata for each song.
We processed the data by aggregating monthly streams to ensure the model could capture patterns across time.

##### Model Training:  
The Prophet model was trained on the historical stream data.
The model identifies three key components:
Trend: Long-term growth or decline in streams.
Weekly Seasonality: Patterns across the days of the week.
Yearly Seasonality: Seasonal patterns across the year (e.g., spikes during holidays or special events).

##### Forecasting:  
We forecasted streams for the next 5 years (2024-2029).
The model predicts an upward trend in streams over time, with seasonal fluctuations captured in the weekly and yearly components.

##### Confidence Intervals:  
The shaded areas in the forecast represent 95% confidence intervals, giving us a range of potential outcomes based on historical variability.

##### Key Insights:  
The overall trend is positive, suggesting steady growth in Spotify streams over the forecast period.
We observe significant fluctuations weekly (higher streams on Thursdays/Fridays) and yearly, which aligns with known streaming behavior patterns.

#### Step 5: Evaluate the Model

## Conclusion

