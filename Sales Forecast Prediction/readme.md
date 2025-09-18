# 📈 Sales Forecast Prediction Using Python

## 🗓️ Last Updated: 23 Jul, 2025

## 📌 Overview
Sales forecasting is a critical component of business strategy, enabling organizations to anticipate future sales and make informed decisions regarding inventory, marketing, and resource allocation. This project demonstrates how to build a predictive model using Python to estimate future sales based on historical data trends.

## 🔍 Project Workflow

### 1. Required Libraries
The project utilizes popular Python libraries for data manipulation, visualization, and machine learning, including:
- pandas
- matplotlib
- seaborn
- scikit-learn
- xgboost

These tools collectively support data preprocessing, feature engineering, model training, and performance evaluation.

### 2. Dataset
The model is trained on a structured sales dataset containing fields such as:
- Row ID
- Order ID
- Customer ID
- Order Date
- Sales

This dataset serves as the foundation for time series analysis and predictive modeling.

### 3. Data Preprocessing & Visualization
- The "Order Date" column is converted to datetime format to enable time-based operations.
- Sales data is aggregated by date to create a daily sales time series.
- A line plot visualizes sales trends over time, highlighting seasonal patterns and fluctuations.

### 4. Feature Engineering
Lagged features are created to capture temporal dependencies in the sales data. These features allow the model to learn from previous sales values and improve forecasting accuracy.

### 5. Data Preparation
- The dataset is split into features and target variables.
- A chronological train-test split ensures the integrity of the time series structure, with 80% of data used for training and 20% for testing.

### 6. Model Training
An XGBoost regression model is trained using the prepared data. Key parameters include:
- Objective: Regression with squared error
- Learning rate: 0.1
- Number of estimators: 100
- Maximum tree depth: 5

XGBoost is chosen for its robustness and ability to model complex patterns in time series data.

### 7. Model Evaluation
- Predictions are made on the test set.
- Root Mean Squared Error (RMSE) is calculated to assess model performance.
- An RMSE of 734.63 indicates a reasonable level of accuracy given the scale of the sales data.

### 8. Results Visualization
A comparison plot of actual vs. predicted sales illustrates the model’s effectiveness. The close alignment between the two curves confirms the model’s ability to capture sales dynamics.

## ✅ Conclusion
This project showcases the power of machine learning in sales forecasting. By leveraging historical data and advanced algorithms like XGBoost, businesses can enhance their decision-making processes, optimize inventory, and improve demand planning.
