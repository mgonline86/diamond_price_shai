# Diamond Price Prediction Model - ShAI Kaggle Competition

## Overview

This repository contains a Jupyter Notebook used for predicting diamond prices as part of the [ShAI Kaggle Competition](https://www.kaggle.com/competitions/diamond-price-prediciton-2024). The goal of the competition was to create a regression model to accurately predict the prices of diamonds based on various features.

### 👉[HTML View](https://mgonline86.github.io/diamond_price_shai/)

## Table of Contents

1. [Introduction](#introduction)
2. [Dataset](#dataset)
3. [Preprocessing](#preprocessing)
4. [Modeling](#modeling)
5. [Evaluation](#evaluation)
6. [Results](#results)
7. [Conclusion](#conclusion)
8. [Supervisor and Team Members](#supervisor-and-team-members)

## Introduction

Diamond pricing can be complex, considering various attributes such as carat, cut, color, clarity, and dimensions. This notebook explores data preprocessing, feature engineering, and model building to predict diamond prices effectively.

## Dataset

The dataset used in this competition includes the following features:

- `carat`: Weight of the diamond.
- `cut`: Quality of the cut (Fair, Good, Very Good, Premium, Ideal).
- `color`: Diamond color, from J (worst) to D (best).
- `clarity`: A measure of diamond clarity (I1, SI2, SI1, VS2, VS1, VVS2, VVS1, IF).
- `depth`: Total depth percentage.
- `table`: Width of the top of the diamond relative to the widest point.
- `x`: Length in mm.
- `y`: Width in mm.
- `z`: Depth in mm.
- `price`: Price of the diamond (target variable).

## Preprocessing

Data preprocessing steps include:

- Handling wrong values.
- Handling Outliers.
- Feautre Engineering (`volume`) from dimensional features (`x`, `y`, `z`).
- Encoding categorical features (`cut`, `color`, `clarity`).
- Feature scaling for numeric variables (`carat`, `depth`, `table`, `volume`).
- Splitting the data into training and testing sets.

## Modeling

We experimented with various regression models including:

- Linear Regression
- Decision Tree Regressor
- K Nearest Neighbor Regressor
- XGBoost Regressor
- Random Forest Regressor

Hyperparameter tuning was performed using `GridSearchCV` to find the best model.

## Evaluation

The model's performance was evaluated using the Root Mean Squared Error (RMSE).

## Results

- **Model Used**: RandomForestRegressor
- **Best Hyperparameters**: {'n_estimators': 200, 'max_features': 3}
- **Final RMSE**: 531.00

## Conclusion

Participating in the ShAI Kaggle Competition provided valuable insights into regression modeling and hyperparameter tuning. While there is room for improvement, our model performed reasonably well, placing us 24th out of 56 teams.

## Supervisor and Team Members

- **Supervisor**:

    Saad Altamari
- **Team**:

    Mohamed Gamal

    Amira Djaiz

    Aya Abu Dabbur

    Mai Serry

    Dyaa Dwekat
