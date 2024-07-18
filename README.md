# Health Trend Prediction of Abnormal Test Results Using LSTM

This project aims to predict the percentage of abnormal test results over time using a Long Short-Term Memory (LSTM) model. The steps involved include data preparation, feature engineering, model training, and evaluation. This repository contains the necessary code and instructions to reproduce the results.

## Table of Contents
1. [Introduction](#introduction)
2. [Data Preparation](#data-preparation)
3. [Feature Engineering](#feature-engineering)
4. [Model Training](#model-training)
5. [Model Evaluation](#model-evaluation)
6. [Results](#results)
7. [Dependencies](#dependencies)


## Introduction

This project focuses on predicting the percentage of abnormal test results for patients over time using an LSTM model. The dataset used contains medical records with various attributes, including patient demographics, medical conditions, and test results.


## Data Preparation

First, we aggregate the data by time intervals (e.g., monthly) and prepare it for time series forecasting.

### Steps:

1. **Load and Clean Data**: Ensure the dataset is cleaned and ready for analysis.
2. **Convert Date Columns**: Convert date columns to datetime format.
3. **Extract Time Features**: Extract month and year from the admission date.
4. **Define Age Groups**: Create bins for age groups.
5. **Aggregate Data**: Group data by year and month, and calculate the percentage of abnormal test results.
6. **Create Time Series**: Set the date as the index for time series analysis.



## Feature Engineering

Generate lag features and prepare train/test datasets.

### Steps:

1. **Create Lag Features**: Generate lag features to capture temporal dependencies.
2. **Split Data**: Split the data into trainig and testing sets.
3. **Reshape Data**: Reshape the data for the LSTM model.



## Model Training

Define and train the LSTM model.

### Steps:

1. **Define Model**: Create the LSTM model architecture.
2. **Compile Model**: Compile the model with appropriate loss function and optimizer.
3. **Train Model**: Train the model using the training data.



## Model Evaluation

Predict and evaluate the model.

### Steps:

1. **Make Predictions**: Predict using the test dataset.
2. **Plot Results**: Visualize the actual vs predicted values.
3. **Compute Metrics**: Calculate evaluation metrics such as MSE, MAE, and R-squared.


## Results

The model was evaluated using the Mean Squared Error (MSE), Mean Absolute Error (MAE), and R-squared metrics. The results indicate the performance of the model in predicting the percentage of abnormal test results over time.


## Dependencies

- pandas
- numpy
- matplotlib
- sklearn
- keras
- tensorflow


This documentation provides a comprehensive overview of your project, guiding users through the steps needed to understand, reproduce, and evaluate the results. Adjust any specific details like the repository URL, your name, and contact information as necessary.
