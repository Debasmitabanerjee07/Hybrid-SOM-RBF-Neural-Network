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
- Performance evaluation using MSE, RMSE, R² Score

## Technologies Used
- Python · MiniSom · Scikit-learn · NumPy · Matplotlib · Pandas

## Key Feature: Data Leakage Prevention
A critical aspect of this project is the strict prevention of data leakage.
Spending Score is included as a feature during SOM training only, so the map
can learn customer topology across all three dimensions. It is fully excluded
from the RBF prediction input — ensuring the model genuinely generalizes to
new data where spending behaviour is unknown.

## Results & Evaluation
The model demonstrates meaningful predictive capability using only two raw attributes (Age and Annual Income):
- R² Score: 0.571 (The model explains 57.1% of the variance in spending)
- RMSE: 14.54 (Predictions are off by ~14.5 points on a 1-100 scale)
- MSE: 211.53

## Dataset
Mall Customers Dataset

## How to Run
1. Clone this repository
2. Install dependencies: `pip install pandas numpy matplotlib seaborn scikit-learn minisom scipy`
3. Open Hybrid_SOM_RBF_Customer_Segmentation.ipynb in Jupyter or Google Colab
4. Run all cells in order

## Author
Debasmita Banerjee
2nd yr. student of Bsc. Data Science
Bhawanipur Global Campus
