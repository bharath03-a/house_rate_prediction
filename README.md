# Kaggle House Price Prediction

This repository contains a comprehensive pipeline for predicting house prices based on the Kaggle competition [House Prices - Advanced Regression Techniques](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques).

## Table of Contents

1. [Introduction](#introduction)
2. [Data Overview](#data-overview)
3. [Exploratory Data Analysis](#exploratory-data-analysis)
4. [Feature Engineering](#feature-engineering)
5. [Modeling](#modeling)
6. [Evaluation](#evaluation)
7. [Submissions](#submissions)
8. [Dependencies](#dependencies)

## Introduction

The project aims to predict house prices using advanced regression techniques. The workflow includes data preprocessing, exploratory data analysis (EDA), feature engineering, and modeling with multiple algorithms to achieve competitive performance.

## Data Overview

The project utilizes the following datasets:
- `train.csv`: Training dataset with house features and target prices.
- `test.csv`: Test dataset with house features.
- `sample_submission.csv`: Sample submission format.

Additional files:
- `data_description.txt`: Detailed explanation of the dataset columns.
- `label_encoded_train.csv` and `label_encoded_test.csv`: Label encoded versions of the datasets.
- `onehot_encoded_train.csv` and `onehot_encoded_test.csv`: One-hot encoded versions of the datasets.

## Exploratory Data Analysis

EDA steps are documented in `eda.ipynb`. Key insights include:
- Visualizing feature distributions and their correlations with the target variable.
- Identifying missing values and handling them appropriately.
- Exploring feature importance.

## Feature Engineering

The `transformation.ipynb` details feature engineering techniques such as:
- Handling missing values.
- Log transformations for skewed features.
- Encoding categorical variables using label encoding and one-hot encoding.
- Dimensionality reduction using PCA.

## Modeling

The `modeling.ipynb` and other notebooks explore multiple models, including:
- Ridge Regression
- LightGBM
- Blended Models

Parameter tuning and blending techniques are applied for optimal performance.

## Evaluation

Models are evaluated based on:
- Root Mean Squared Error (RMSE)
- Performance on the leaderboard (using Kaggle's private and public splits).

## Submissions

Submission files are saved in the `submissions/` directory, including:
- `submission.csv`
- `submission_lightgbm.csv`
- `submission_ridge.csv`
- Blended and PCA-enhanced submissions.

## Dependencies

The project relies on the following Python libraries:
- `numpy`
- `pandas`
- `matplotlib`
- `seaborn`
- `scikit-learn`
- `lightgbm`
