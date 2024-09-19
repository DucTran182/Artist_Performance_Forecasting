# Artist_Performance_Forecasting

## Table of Contents
1. [Introduction](#introduction)
2. [Setup and Installation](#setup-and-installation)
3. [The Process](#the-process)
4. [Run The Code](#run-the-code)
5. [Conclusion](#conclusion)

## Introduction
This project is to design a performance forecasting model for the singer "ISAAC," predicting his growth over the next five years (2024-2029) on platforms like YouTube and Spotify. The ISAAC performance forecasting model aims to predict the future trajectory of his music career, focusing on YouTube and Spotify metrics. The result will guide investment decisions for a company seeking to capitalize on ISAAC’s potential growth.

## Setup and Installation
To run the model locally, follow these steps:

1. Install python3.11.9.
2. Set up Jupyter Notebook development environment (pip install pandas, matplotlib, scikit-learn, statsmodels, prophet)
3. Clone this repository.
4. Download dataset

## The Process
##### Model Selection:  
I used Facebook Prophet, a robust time series forecasting model. Prophet is well-suited for capturing trends and seasonality in streaming data due to annual music trends and release cycles, making it ideal for predicting future performance. Especially, it is relatively easy to implement and interpret and have fewer hyperparameters to tune compared to more complex models.

##### Data Preparation:  
The dataset includes Spotify stream data and YouTube views data from 2017 to September 2024, along with key metadata for each song.
I processed the data by aggregating monthly streams to ensure the model could capture patterns across time.

##### Model Training:  
The Prophet model was trained on the historical stream data. The model identifies three key components:  
Trend: Long-term growth or decline in streams.  
Weekly Seasonality: Patterns across the days of the week.  
Yearly Seasonality: Seasonal patterns across the year (e.g., spikes during holidays or special events).

##### Trend Analysis:  
The model identified an upward trend in streams over time, indicating potential growth. This is visualized in the trend component, where the stream counts are predicted to increase steadily until 2029.

##### Seasonal Patterns:  
Weekly Seasonality: Significant spikes are observed on Sundays and Thursdays, showing user activity patterns by the day of the week.  
Yearly Seasonality: We noticed periodic fluctuations in streams during specific months, such as peaks around February and drops in late December.

##### Forecasting:  
I forecasted streams for the next 5 years (2024-2029).
The model predicts an upward trend in streams over time, with seasonal fluctuations captured in the weekly and yearly components. The blue line in the forecast chart represents the expected stream values, while the shaded region indicates confidence intervals. 

##### Confidence Intervals:  
The shaded areas in the forecast represent 95% confidence intervals, giving me a range of potential outcomes based on historical variability.

## Run the code
After installing everything, you just need to run the main.ipynb to get the forecasting results of ISAAC's performance on Spotify and YouTube. 
P/s: I have already converted the data from spreadsheet to CVS format.

To run, follow these 4 steps:
#### Step 1: Load data into the code  
#### Step 2: EDA to understand its structure and distribution as well as to prepare and transform for modeling     
#### Step 3: Visualize the data to get an overview before forecasting with matplotlib.pyplot  
#### Step 4: Build a forecasting model with Prophet  
#### Step 5: Evaluate the Model

## Conclusion  
### Key Insights:
##### The Long-term Trend:  
The model predicts a gradual increase in Spotify streams over the next 5 years, indicating that ISAAC's popularity is expected to grow in this platform. This is a positive signal for long-term investment. On the other hand, his performance on YouTube significantly decreases in the next 5 years. It will be a risky investment on this platform.

##### Seasonality Patterns:  
The weekly and yearly seasonality highlight predictable fluctuations in user behavior. Spikes in streams on certain days and during specific months can be leveraged for marketing campaigns, new releases, or promotions. For example, higher Spotify streams on Sundays and Thursdays, whereas higher YouTube views on Sunday only, suggest targeted marketing or release strategies on those days to maximize engagement.

##### Uncertainty and Variability:   
While there is a positive and negative growth trends, the confidence intervals show potential volatility. It suggests being cautious with high-risk investments and using flexible strategies that can adapt to these fluctuations. Monitor the actual stream performance closely against forecasted values.

### Business Decision Recommendations:
##### Increased Investment:   
Given the overall positive growth forecast, consider increasing marketing efforts and investments to capitalize on ISAAC’s expected rising popularity in Spotify.

##### Strategic Releases:   
Plan song releases, promotional campaigns, or collaborations with peak streaming days (Sundays and Thursday) and months to maximize reach and impact. Publishing on Sunday if the company wants to upload on YouTube.

##### Risk Management:  
While growth is expected, monitor market changes closely, especially around the times of variability shown in the forecast. Reassess the forecast periodically (e.g., every 6 months) to ensure the model is performing as expected. Consider diversification strategies to minimize risk during volatile periods.
