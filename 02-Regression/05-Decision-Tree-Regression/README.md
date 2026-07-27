# Decision Tree Regression

## Overview

Decision Tree Regression is a non-linear regression algorithm that makes predictions by repeatedly splitting the dataset into smaller groups based on decision rules. These splits form a tree-like structure, where each branch represents an if-else condition that helps minimise prediction error.

Unlike regression models that fit a mathematical equation, Decision Tree Regression learns how to split the data into different regions before making predictions. Another key characteristic of this algorithm is that it does not require feature scaling, making it simpler to prepare the data before training the model.

## Dataset

This implementation uses the **Position_Salaries** dataset.

- **Independent Variable (X):** Position Level
- **Dependent Variable (y):** Salary

## What You'll Find Here

- Trained a Decision Tree Regression model using Scikit-learn
- Predicted the salary for a new position level
- Visualised the fitted Decision Tree Regression model
