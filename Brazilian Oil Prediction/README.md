# 🛢 Monthly Oil Production Forecast

A project that leverages both Linear Regression and the Prophet library to forecast monthly oil production.

## 📋 Table of Contents
- [Introduction](#introduction)
- [Dataset](#dataset)
- [Problem Statement](#problem-statement)
- [Data Processing](#data-processing)
- [Methodologies](#methodologies)
- [Model Scores](#model-scores)
- [Visualization](#visualization)
- [Deployment with FastAPI](#deployment-with-fastapi)
- [Usage](#usage)

## 📌 Introduction
This project aims to predict monthly oil production values using two main methodologies: Linear Regression and Facebook's Prophet Library.

## 🗃 Dataset
The dataset used in this project is available at the following URL:
[Dataset on Kaggle](https://www.kaggle.com/code/erivanoliveirajr/predict-of-future-oil-production)

## 📝 Problem Statement
Based on Petrobras' mercantile strategies, it's advantageous to sell certain oil fields to companies interested in purchasing them. Therefore, there's an interest in predicting the oil production of these fields using Time Series analysis.

## 🔄 Data Processing
The dataset undergoes several transformations:
* Aggregating monthly oil production values.
* Adjusting DateTime formatting.
* Deriving various metrics including trends and lags.

## 🧪 Methodologies
### 📉 Linear Regression Model
This method employs a Linear Regression model to forecast monthly oil production. Each forecasted month's value is then re-integrated into the dataset for subsequent predictions. Here's an insight into the results achieved using the model:
* **Intercept:** 4059402.3957887287
* **Regression Score:** 0.9705558174249665

### 📊 Prophet Forecasting
The Prophet library is harnessed to project monthly oil production for the subsequent 24 months, supplemented with visual insights into its components, notably the trend.

## 📈 Model Scores
Evaluation metrics for the Prophet model are as follows:
- **Mean Squared Error (MSE):** 46639961341.9966
- **Mean Absolute Error (MAE):** 177165.8899606352
- **Mean Absolute Percentage Error (MAPE):** 0.05032680609149977
- **R-squared (R2):** 0.9570427032705945

## 🖼 Visualization
The results are illustrated through:
- Comparisons between original and predicted values.
- Confidence intervals highlighting the upper and lower bounds of predictions.

## 🚀 Deployment with FastAPI
The fine-tuned Linear Regression model is geared up for deployment via FastAPI. This deployment ensures user-friendly access for generating monthly oil production predictions.

## 🔍 Usage
The FastAPI endpoint is primed for prediction. Simply input the requisite parameters, and the endpoint furnishes the forecasted monthly oil production.

