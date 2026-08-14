# Random Forest Classification

## Overview

Random Forest Classification is a supervised machine learning algorithm that combines the predictions of multiple Decision Trees to make a final classification. By aggregating the results of several trees, the model can produce more robust predictions than relying on a single Decision Tree.

In this notebook, I trained a Random Forest Classifier using Scikit-learn to predict whether a user will purchase an SUV based on their age and estimated salary. The model was configured with `n_estimators = 10`, meaning that 10 Decision Trees were trained and their predictions were combined to determine the final class.

The `entropy` criterion was used to evaluate the quality of splits within each tree, favouring splits that produce purer groups. Increasing the number of trees can generally make the model more stable and robust, although it also increases computational cost.

Although feature scaling is included in the classification preprocessing pipeline, it is not required for Random Forests because the underlying Decision Trees make decisions using feature thresholds rather than distances or feature magnitudes.

## Dataset

This implementation uses the Social_Network_Ads dataset.

- **Independent Variables (X):** Age, Estimated Salary
- **Dependent Variable (y):** Purchased (0 = No, 1 = Yes)

## What You'll Find Here

- Splitting the dataset into training and testing sets
- Training a Random Forest Classifier using 10 Decision Trees
- Using entropy to evaluate the quality of tree splits
- Predicting whether a new user will purchase an SUV
- Evaluating the model using a confusion matrix and accuracy score
- Visualising the decision boundary on the training and test sets

## Results

The Random Forest Classifier achieved an accuracy of **91%** on the test set.

The decision boundary remains composed of distinct, threshold-based regions because the Random Forest is built from Decision Trees. However, combining multiple trees produces a more complex and robust classification boundary than a single Decision Tree.

For comparison, the models implemented in this classification section achieved:

- **Logistic Regression:** 89%
- **K-NN:** 93%
- **SVM (Linear):** 90%
- **Kernel SVM (RBF):** 93%
- **Naive Bayes:** 90%
- **Decision Tree:** 91%
- **Random Forest:** 91%

On this dataset and test split, K-NN and Kernel SVM achieved the highest accuracy at 93%, while the Random Forest matched the Decision Tree at 91%.
