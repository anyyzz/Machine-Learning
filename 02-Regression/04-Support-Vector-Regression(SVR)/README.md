# Support Vector Regression (SVR)

## Overview

Support Vector Regression (SVR) is a non-linear regression algorithm that can model complex relationships between variables using kernel functions. In this implementation, I used the **Radial Basis Function (RBF) kernel** to capture the non-linear relationship between position level and salary.

Unlike the previous regression models, **SVR requires feature scaling for both the independent variables (X) and the dependent variable (y)**, as the algorithm is based on distances between data points. After training the model, the predictions were transformed back to the original scale for interpretation.

## Dataset

This implementation uses the **Position_Salaries** dataset.

- **Independent Variable (X):** Position Level
- **Dependent Variable (y):** Salary

## What You'll Find Here

- Applied feature scaling to both the independent and dependent variables
- Trained an SVR model using the RBF kernel
- Predicted the salary for a new position level
- Converted predictions back to the original scale
- Visualised the fitted regression curve
