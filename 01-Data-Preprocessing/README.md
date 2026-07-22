# Data Preprocessing

## Overview

Data preprocessing is one of the most important stages of a machine learning pipeline. Before a model can learn from data, the dataset must be cleaned and transformed into a format suitable for training. 
This project demonstrates the essential preprocessing techniques commonly applied before building a machine learning model using Scikit-learn.


## Learning Objectives

This project covers the complete preprocessing workflow, including:

- Loading and exploring a dataset
- Separating independent and dependent variables
- Handling missing data
- Encoding categorical variables
- Splitting the dataset into training and testing sets
- Applying feature scaling


## Workflow

### 1. Importing the Required Libraries

The project begins by importing the libraries used throughout the preprocessing pipeline.

- **NumPy** – numerical computations
- **Pandas** – loading and manipulating datasets
- **Matplotlib** – data visualisation
- **Scikit-learn** – preprocessing and machine learning utilities


### 2. Loading the Dataset

The dataset is imported using Pandas and separated into:

- **X** – the independent variables (features)
- **y** – the dependent variable (target)

This allows the model to distinguish between the input data and the values it is expected to predict.


### 3. Handling Missing Values

Real-world datasets often contain missing values.

The `SimpleImputer` is used to replace missing numerical values with the mean of each respective column, ensuring that incomplete data does not negatively affect model training.


### 4. Encoding Categorical Variables

Machine learning algorithms operate on numerical data.

The preprocessing pipeline converts categorical values into numerical representations using:

- **One Hot Encoding** for independent categorical features.
- **Label Encoding** for the dependent variable.


### 5. Splitting the Dataset

The dataset is divided into:

- **Training Set (80%)**
- **Testing Set (20%)**

The training set is used to train the model, while the testing set is reserved for evaluating how well the model performs on unseen data.


### 6. Feature Scaling

Many machine learning algorithms perform better when features are measured on a similar scale.

Feature scaling ensures that features with larger numerical values do not disproportionately influence the learning process.

## Key Learning Outcomes

Through this project, I learned:

- How to prepare raw datasets for machine learning.
- The importance of handling missing values before training a model.
- The difference between One Hot Encoding and Label Encoding.
- Why datasets are split into training and testing sets.
- Why feature scaling is an important step in preparing data for machine learning models.

## Reflection

This project introduced me to the preprocessing pipeline used before training machine learning models. Understanding these preprocessing techniques helped me appreciate how the quality and preparation of data can influence the performance of a machine learning model.
