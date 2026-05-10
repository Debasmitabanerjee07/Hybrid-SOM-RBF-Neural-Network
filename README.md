# Hybrid-SOM-RBF-Neural-Network
Customer Segmentation and Prediction using SOM and RBF Neural Networks

## Overview
This project combines:
- Self-Organizing Maps (SOM)
- Radial Basis Function Networks (RBF)

for customer segmentation and prediction.

## Features
- Data preprocessing and scaling
- SOM-based clustering
- RBF feature transformation
- Prediction using Linear Regression
- Performance evaluation using:
  - MSE
  - RMSE
  - R² Score

## Technologies Used
- Python
- MiniSom
- Scikit-learn
- NumPy
- Matplotlib
- Pandas
##   Key Feature: Data Leakage Prevention
A critical aspect of this project is the strict prevention of data leakage
. While the target "Spending Score" was used during the initial unsupervised SOM phase to help identify natural clusters, it was completely excluded from the input features for the RBF prediction stage
. This ensures the model's performance reflects its ability to generalize to new, real-world data

##   Results & Evaluation
The model demonstrates meaningful predictive capability using only two raw attributes (Age and Annual Income):
- R² Score: 0.571 (The model explains 57.1% of the variance in spending).
- RMSE: 14.54 (Predictions are off by ~14.5 points on a 1-100 scale).
- MSE: 211.53.
The Actual vs. Predicted visualization shows a clear positive trend along the ideal diagonal, confirming that the hybrid architecture successfully learned the relationship between customer demographics and spending behavior
## Dataset
Mall Customers Dataset

## Author
Debasmita Banerjee
Bhawanipur Global Campus- 2nd yr. Bsc.Data Science
