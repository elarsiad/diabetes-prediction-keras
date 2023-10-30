# Diabetes Prediction with Deep Learning

## Overview

This project uses a deep neural network model to predict whether a patient has diabetes based on diagnostic measurements from the Pima Indians Diabetes dataset. The data contains medical records for Pima Indian female patients aged 21 and above.

The model goes through the typical machine learning workflow:

- Data understanding and exploration 
- Data cleaning and preprocessing
- Data modeling with a deep neural network 
- Model evaluation and optimization

## Data Understanding and Exploration

The dataset contains 768 records with 9 features - number of pregnancies, glucose level, blood pressure, skin thickness, insulin level, BMI, diabetes pedigree function, age, and diabetes outcome. 

Exploratory data analysis is performed to understand the features, missing values, outliers, correlations, etc. Visualizations are created to analyze distributions and relationships between features.

## Data Cleaning and Preprocessing

Columns with excessive missing values are dropped. Remaining missing values are imputed appropriately based on data distributions. Outliers are identified and handled. The data is scaled and normalized. The dataset is balanced using SMOTE oversampling due to class imbalance.

## Modeling

A deep neural network model with dense layers is built in Keras using the TensorFlow backend. The model is trained and validated on the prepared dataset. Callbacks are used for early stopping.

## Evaluation

The model is evaluated on various performance metrics like accuracy, AUC, sensitivity, specificity etc. The threshold for classification is optimized to balance sensitivity and specificity.

## Conclusion

The deep learning model is able to predict diabetes with good performance, achieving over 80% accuracy on the test set. The model can be further improved and deployed for real-world use.