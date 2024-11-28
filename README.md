# Settlement Prediction of Clayey Soils using Machine Learning

## Project Overview

This project focuses on predicting the settlement characteristics of clayey soils using machine learning techniques. The goal is to accurately predict the settlement of clayey soils under specific loading conditions by utilizing a dataset consisting of various soil properties. Several machine learning models are employed to analyze soil behavior and predict settlement, including **Support Vector Regression (SVR)**, **Multi-layer Perceptron (MLP)**, and **XGBoost**.

The dataset used in this project was derived from multiple sources, with the final settlement being calculated using **Terzaghi’s consolidation theory**, assuming a height of **1 meter** and a load of **100 kPa**. The models are trained and evaluated using this dataset to explore the best-performing machine learning approach for soil settlement prediction.

## Dataset

The dataset used in this project consists of empirical data on clayey soils, sourced from various research studies:

- **Basma et al. (1994)**
- **Hakami and Abu Seif (2019)**
- **Çimen (2002)**
- **Tonoz (2003)**

Additionally, the dataset was extended using an empirical formula for the void ratio based on water content, as described in the article by **Obaji et al. (2020)**.

The dataset includes the following features (input variables):
- Clayey soil fraction (gravel, silt, sand, clay fraction)
- Bulk density
- Atterberg limits (Liquid limit, Plastic limit, etc.)
- Void ratio
- Compression index (Cc)
- Water content
- Swelling pressure

The target variable for this project is the **settlement** (denoted as **S**).

## Models Used

This project investigates the performance of the following machine learning models to predict the settlement of clayey soils:

1. **Support Vector Regression (SVR)**
   - SVR is a regression technique derived from Support Vector Machines (SVM), designed to find a function that approximates the given data within a specified tolerance.

2. **Multi-layer Perceptron (MLP)**
   - MLP is a neural network model consisting of multiple layers of neurons, capable of learning complex nonlinear relationships through backpropagation.

3. **XGBoost**
   - XGBoost is an optimized gradient boosting algorithm, known for its speed and performance, particularly in handling large datasets and capturing intricate patterns.

The models are evaluated using **5-fold cross-validation** to ensure robustness in their predictions.

## Results

The models were trained and evaluated using the dataset. The results showed the following:

- **SVR Model**: This model demonstrated a strong ability to capture the nonlinear relationships in the data. However, its performance was slightly less accurate when compared to the other models.

- **MLP Model**: The MLP model provided competitive results, showing good performance in modeling complex nonlinear relationships. It performed well, but not as accurately as XGBoost.

- **XGBoost Model**: XGBoost outperformed the other models, providing the most accurate predictions for settlement. Its ability to handle complex relationships and prevent overfitting contributed to its superior performance.

The models' performance was evaluated using metrics such as Mean Squared Error (MSE), R², and residual plots. The results indicated that all models performed reasonably well, but XGBoost emerged as the most effective model for predicting the settlement of clayey soils.
