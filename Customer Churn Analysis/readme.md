# 🔄 Customer Churn Analysis Prediction

## 🗓️ Last Updated: 20 Aug, 2025

## 📌 Overview
Customer churn refers to the phenomenon where customers discontinue using a company’s services, leading to potential revenue loss. Understanding churn patterns is essential for businesses to improve customer retention and long-term growth. This project leverages the Telco Customer Churn dataset to build a predictive model that identifies customers likely to churn.

## 🧠 Objective
The goal is to analyze customer behavior and predict churn using machine learning techniques. By identifying at-risk customers, businesses can take proactive measures to enhance satisfaction and reduce attrition.

## 🔍 Project Workflow

### 1. Dataset Overview
The dataset includes customer details such as:
- Tenure with the company
- Internet service type
- Payment method
- Churn status (Yes/No)

Initial steps involve loading the dataset, inspecting its structure, and visualizing churn distribution to understand class balance.

### 2. Data Preprocessing
Key preprocessing steps include:
- **Handling Missing Values**: Converting non-numeric entries in `TotalCharges` to numeric and filling missing values with the median.
- **Encoding Categorical Variables**: Transforming categorical features into numerical format using label encoding.
- **Feature Selection**: Removing irrelevant columns like `customerID` and separating features from the target variable (`Churn`).
- **Train-Test Split**: Dividing the dataset into training and testing sets (80/20 split).
- **Feature Scaling**: Standardizing features to ensure uniformity and improve model performance.

### 3. Model Training
A **Random Forest Classifier** is used for prediction. This ensemble method combines multiple decision trees to improve accuracy and reduce overfitting. The model is trained on the standardized training data.

### 4. Model Evaluation
- **Accuracy Score**: The model achieves an accuracy of 78%, indicating reasonable performance.
- **Confusion Matrix**: Provides insights into true positives, true negatives, false positives, and false negatives. While the model correctly identifies many churners and non-churners, a notable number of churners are missed, suggesting room for improvement.

### 5. Insights & Recommendations
- The model performs well but could benefit from hyperparameter tuning or alternative algorithms to reduce false negatives.
- Understanding feature importance can guide business strategies to retain customers more effectively.

## ✅ Conclusion
This project demonstrates how machine learning can be applied to predict customer churn, enabling businesses to make data-driven decisions. With further refinement, such models can become powerful tools for customer retention and strategic planning.
