# Customer Churn Analysis in Iranian Telecom Dataset

## ⭐ Project Summary

This project explores the **customer churn behavior** of a telecom company using Exploratory Data Analysis (EDA) and basic classification modeling. The dataset contains 3,150 customer records and 14 attributes. It was part of a practice case for a Data Scientist certification exam. 

_📝 Note: This notebook is written in Bahasa Indonesia for educational purposes (certification practice). However, the overall documentation and project structure are described in English._

## 📁 Dataset
[![UCI Dataset](https://img.shields.io/badge/UCI%20Dataset-Iranian%20Churn-orange?logo=data)]([https://archive.ics.uci.edu/dataset/563/iranian+churn+dataset](https://archive.ics.uci.edu/dataset/563/iranian+churn+dataset))

### ⭐ Situation
Customer churn is one of the major concerns for subscription-based businesses, including telecom providers. Losing customers without clear behavioral insights can lead to revenue loss and poor service planning.

The dataset used in this project comes from an Iranian telecom company, containing numerical customer attributes such as call usage, complaints, age, and value metrics.

### ⭐ Task
The main goal was to:
- Perform **descriptive and exploratory analysis** to understand patterns in churn behavior.
- Identify key variables that influence customer churn.
- Train a **basic classification model (Decision Tree)** to predict whether a customer will churn or stay.
- Evaluate model performance and interpret confusion matrix results.

### ⭐ Action
- Cleaned and explored the dataset (no missing values, all numerical columns).
- Performed descriptive statistics and visualized distributions for all features.
- Analyzed class imbalance (churn = 15.7%, non-churn = 84.3%).
- Created correlation matrix and boxplots to identify significant predictors.
- Trained a **Decision Tree Classifier**, and later optimized it using hyperparameter tuning.
- Evaluated model performance using accuracy, precision, recall, and F1-score.

### ⭐ Result
- Found that **Complaints** and **Status** had strong positive correlation with churn, while features like **Customer Value** and **Usage** had negative correlation.
- Initial model achieved:
  - **Accuracy**: 93.5%
  - **Precision (churn class)**: 0.79
  - **Recall (churn class)**: 0.80
- After tuning:
  - Accuracy = **93.3%**
  - Model was more stable but **less effective in detecting churn cases**.
- Insights:
  - Churners tend to have fewer SMS, lower usage time, and are more likely to have filed complaints.
  - Class imbalance affected prediction performance for minority class (churn).
  - Suggested next step: SMOTE or other class-balancing methods.
 
