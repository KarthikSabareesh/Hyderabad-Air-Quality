# Hyderabad-Air-Quality
An exercise to predict air quality in Hyderabad in COVID affected time, from October 2019 to April 2020

## We undergo multiple data and moodel processing steps to try to achieve a satisfactory Air Quality Prediction Model, which include data cleaning, imputation, feature engineering, varation and outlier visualisation, hyperparameter tuning, etc.

## A) Data Processing Steps (Data Cleaning and Feature Engineering):

### 1) Outlier Removal( via IQR method).
### 2) Mutual Information Scoring of features to evaluate to aid in feature selection for evalutating models.
### 3) Principal Component Analysis (PCA) of initial features for usage as new features, analysis of variation and dimensionality reduction.
### 4) Unsupervisied learning via Clustering (HDBSCAN) for deeper analysis, usage as feature and dimensionality reduction.

## B) Model Steps:

### 1) Trial of 4 different regression models (RandomForest,XGBoost,LightGBM,SVM Regressor)
### 2) Analysis of model performance in each data processing step
### 3) Hyperparameter Tuning for chosen model type via RandomizedSearchCV

#### Note 1:  HDBSCAN is an advanced, hierarchal density based clustering algorithm that I chose to try to find the most efficient clustering method possible, which proved to be a huge factor in dimensionality reduction in the later steps
#### Note 2: Here, PCAs produced lesser no. of values than original features and had to be imputed and corrected for length before being added to the data it was derived from to try and pick the best combination of original and PCA features.
#### Note 3 : The final model type which was selected was done so after careful consideration of each model type's performance in roughly default conditions on the datset. RandomizedSearchCV was performed for a couple other model types as well, but were'nt represented in this notebook in the interest of keeping the notebook concise and short, as they returned relatively worse results compared to the best model type

## Thank You for Reading!!! 
