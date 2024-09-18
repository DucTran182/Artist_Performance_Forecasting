# Artist_Performance_Forecasting

## Table of Contents
1. [Introduction](#introduction)
2. [Setup and Installation](#setup-and-installation)
3. [Run The Code](#run-the-code)

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
(P/s: I have converted the data from spreadsheet to CVS format.)

#### To run, follow these 4 steps:
Step 1: Load data into the code

Step 2: EDA to understand its structure and distribution as well as to prepare and transform for modeling 

Step 3: Visualize the data to get an overview before forecasting with matplotlib.pyplot

Step 4: Build a forecasting model with Prophet 
P/s: I chose Prophet model because Prophet is designed to handle seasonality and trends in time series data. It’s particularly effective for data with strong yearly or weekly seasonal patterns, which can be common in streaming and viewership data due to annual music trends and release cycles. Especially, it is relatively easy to implement and interpret and have fewer hyperparameters to tune compared to more complex models.

Step 5: Evaluate the Model

Once this model is deployed, it can be retrained with updated data every few months to ensure accuracy.


