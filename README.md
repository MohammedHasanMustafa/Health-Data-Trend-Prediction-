# Time Series Prediction of Abnormal Test Results Using LSTM

This project aims to predict the percentage of abnormal test results over time using a Long Short-Term Memory (LSTM) model. The steps involved include data preparation, feature engineering, model training, and evaluation. This repository contains the necessary code and instructions to reproduce the results.

## Table of Contents
1. [Introduction](#introduction)
2. [Data Preparation](#data-preparation)
3. [Feature Engineering](#feature-engineering)
4. [Model Training](#model-training)
5. [Model Evaluation](#model-evaluation)
6. [Results](#results)
7. [Usage](#usage)
8. [Dependencies](#dependencies)
9. [Author](#author)
10. [License](#license)

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
