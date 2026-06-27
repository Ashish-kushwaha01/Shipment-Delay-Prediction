# Shipment Delay Prediction

## Overview

This project predicts the number of shipment delay days using various Machine Learning regression algorithms. The objective is to build a predictive model that estimates shipment delays based on project and shipment-related features.

Several regression models were trained, compared, and evaluated using Mean Absolute Error (MAE). Hyperparameter tuning was also performed to improve model performance.

---

## Project Workflow

### 1. Data Loading

- Loaded the dataset using Pandas.
- Inspected the dataset structure.
- Checked data types and missing values.

### 2. Data Cleaning

- Removed duplicate records.
- Handled missing values (if any).
- Verified dataset consistency.

### 3. Exploratory Data Analysis (EDA)

Performed exploratory analysis to understand the dataset.

- Statistical summary
- Feature distributions
- Correlation analysis
- Outlier detection using the IQR method

### 4. Outlier Handling

Detected outliers using the Interquartile Range (IQR) method.

- Identified outliers in numerical columns
- Applied outlier treatment where necessary

### 5. Feature Engineering

Prepared the dataset for model training by:

- Selecting relevant features
- Separating independent and dependent variables

### 6. Train-Test Split

Split the dataset into training and testing sets.

- Training Set: 80%
- Testing Set: 20%

### 7. Model Training

The following regression models were trained:

- Linear Regression
- Decision Tree Regressor
- Random Forest Regressor
- Tuned Random Forest Regressor
- Gradient Boosting Regressor
- XGBoost Regressor

### 8. Hyperparameter Tuning

Performed hyperparameter tuning using GridSearchCV for:

- Random Forest Regressor

Parameters tuned:

- n_estimators
- max_depth
- min_samples_split

### 9. Model Evaluation

All models were evaluated using:

- Mean Absolute Error (MAE)

The MAE values of all models were compared using a bar chart.

## Results

After comparing all regression models using MAE, Linear Regression achieved the lowest Mean Absolute Error on this dataset.

This indicates that the relationship between the input features and the target variable is largely linear, allowing the simpler Linear Regression model to generalize better than the more complex ensemble methods.

---

## Author

Ashish Kushwaha
