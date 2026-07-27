# Random Forest Regression

## Overview

Random Forest Regression is a non-linear ensemble learning algorithm that combines the predictions of multiple Decision Trees to produce a more robust model and often improve prediction accuracy. Instead of relying on a single tree, it builds a collection of trees and averages their predictions to reduce the risk of overfitting.

The number of trees used in the model is controlled by the **`n_estimators`** parameter. In this implementation, I used **10 decision trees** (`n_estimators = 10`) to predict salaries based on position level using Scikit-learn.

## Dataset

This implementation uses the **Position_Salaries** dataset.

- **Independent Variable (X):** Position Level
- **Dependent Variable (y):** Salary

## What You'll Find Here

- Trained a Random Forest Regression model using Scikit-learn
- Predicted the salary for a new position level
- Visualised the fitted Random Forest Regression model
