# M5-Forecasting-Accuracy
This repo contains code used for m5 forecasting accuracy that happened in Kaggle from March to June 2020. The link to the competetion is found [here](https://www.kaggle.com/c/m5-forecasting-accuracy).

I published an Medium article clearly explaining my work for these project and interested people can read it from [here](https://towardsdatascience.com/m5-forecasting-accuracy-24d7f42130de).

In this notebook, the Exploratory Data analysis for M5 competition data is performed using R and sales for 28 days were forecasted using Xgboost, Catboost, Lightgbm, and Facebook prophet. The best model is chosen by comparing the SMAPE error rate and One standard error rule.

## Background of Competition:
The Makridakis Competitions (also known as the M Competitions) are series of open competitions organized by teams led by forecasting researcher Spyros Makridakis and intended to evaluate and compare the accuracy of different forecasting methods. he first competition named M-Competition was held way back in 1982 with only 1001 data points, the complexity of model and data scale increased with every successive iteration.

## Aim:
In March this year(2020), the fifth iteration named M5 competition was held. This m5 competition aims to forecast daily sales for the next 28 days i.e., till 22nd May 2016, and to make uncertainty estimates for these forecasts. In this blog, I am just going to do forecasting and uncertainty will be performed in my next blog with the best-chosen model.

## Dataset:
The dataset provided contains 42,840 hierarchical sales data from Walmart. The dataset covers stores in three US states (California, Texas, and Wisconsin) and includes item level, department, product categories, and store details for 5 years starting from 29th Jan 2011 to 24th April 2016. Also, it has explanatory variables such as price, snap events, day of the week, and special events and festivals.The data comprises 3049 individual products from 3 categories and 7 departments, sold in 10 stores in 3 states. The hierarchical aggregation captures the combinations of these factors which makes it feasible to perform a bottom-up approach or top-down approach. For instance, we can create 1 time series for all sales or perform for each state separately and so on. And datset can be downloaded from [here](https://www.kaggle.com/c/m5-forecasting-accuracy/data)


The models used to forecast sales are Xgboost, Catboost,Lightgbm and facebook prophet. Total Code was written in R languaue and code is uploaded in Jupyter Notebook format.
My kaggle notebook can be accessed directly from [here](https://www.kaggle.com/jaswanthhbadvelu/cat-xgb-lgboost-prophet).
