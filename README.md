# Lasso and Inductive Conformal Prediction Algorithm

## Overview

This repository contains Python code implementing Lasso regression and an Inductive Conformal Predictor for predicting diabetes-related outcomes. The code utilizes the scikit-learn library for Lasso regression and inductive conformal prediction principles.

## Files

- **lasso_diabetes.py**: Python script implementing Lasso regression on the diabetes dataset.
- **lasso_diabetes_tabsep.py**: Python script implementing Lasso regression on a tab-separated diabetes dataset.
- **conformal_prediction.py**: Python script implementing the Inductive Conformal Predictor.
- **README.md**: Overview of the repository and usage instructions.

## Instructions

1. Lasso Regression for diabetes dataset
    - Load the diabetes dataset using `load_diabetes` from sklearn.
    - Split the dataset into training and testing sets.
    - Train Lasso models with different alpha values and assess their performance.
    - Evaluate the number of selected features and their impact on test R2.
    - Visualize the relationship between test R2 and the number of features.

2. Lasso Regression for tab-separated diabetes dataset
    - Read the tab-separated diabetes dataset.
    - Split the dataset into training and testing sets.
    - Train Lasso models with different alpha values and evaluate their performance.
    - Assess the number of selected features and their impact on test R2.
    - Visualize the relationship between test R2 and the number of features.

3. Standard Scaling and Cross-validation
    - Preprocess the training and test sets using StandardScaler.
    - Choose the regularization parameter for Lasso using cross-validation on the training set.

4. **Inductive Conformal Predictor**
    - Split the original training data into new training and calibration data.
    - Preprocess data using StandardScaler.
    - Find the best parameter for Lasso and predict preprocessed calibration data.
    - Calculate non-conformity measures and define significance levels.
    - Predict for scaled test data and calculate prediction intervals.
    - Assess error rates for predicted labels at different significance levels.

## Dependencies

- Python 3.x
- scikit-learn
- pandas
- matplotlib
- numpy

## How to Use

1. Clone the repository:

   ```bash
   git clone https://github.com/your_username/lasso-conformal-prediction.git
   ```

2. Install dependencies:

   ```bash
   pip install scikit-learn pandas matplotlib numpy
   ```

3. Run the Python scripts as needed:

   ```bash
   python lasso_diabetes.py
   python lasso_diabetes_tabsep.py
   python conformal_prediction.py
   ```

Feel free to explore and modify the code to suit your specific needs. For more details, refer to the comments within each script.
