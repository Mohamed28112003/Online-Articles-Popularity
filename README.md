

# Project Title
**Online Articles Popularity Prediction**

# Project Overview
The objective of this project is to predict the popularity of online articles using machine learning techniques. We have built models for both regression (to predict the number of shares) and classification (to categorize articles into popularity classes).

# Table of Contents
- [Introduction](#introduction)
- [Dataset](#dataset)
- [Preprocessing](#preprocessing)
- [Feature Engineering](#feature-engineering)
- [Models](#models)
- [Evaluation](#evaluation)
- [Results](#results)
- [Conclusion](#conclusion)
- [References](#references)

# Introduction
This project aims to analyze various features of online articles and build predictive models to estimate their popularity. The popularity is measured in terms of the number of shares an article receives.

# Dataset
The dataset used for this project contains 38,643 rows and 46 columns, including features such as `timedelta`, `n_tokens_content`, `weekday`, etc. The target variable is the number of shares.

# Preprocessing
- **Handling Missing Values:** We checked for missing data and either removed or filled them appropriately.
- **Duplicates:** No duplicates were found.
- **Outliers:** Outliers were replaced with upper bounds.
- **Encoding:** Categorical features were encoded using one-hot encoding and label encoding.

# Feature Engineering
- Created new features such as `title_length`.
- Extracted important information from columns like `url` and `title`.
- Normalized numerical features.

# Models
- We implemented and compared several models for both regression and classification tasks.

## Regression Models
- Linear Regression
- Random Forest Regressor
- Gradient Boosting Regressor
- XGBoost Regressor

# Classification Models
- Logistic Regression
- Support Vector Machine (SVM)
  - RBF Kernel
  - Polynomial Kernel
- XGBoost Classifier

# Evaluation
- **Regression Models:** Evaluated using Mean Squared Error (MSE) and R-squared (R²) metrics.
- **Classification Models:** Evaluated using accuracy, precision, recall, and F1-score.

# Results
- Regression
  - The XGBoost Regressor provided the best performance with the highest R² score and the lowest MSE.

- Classification
  - The XGBoost Classifier achieved the highest accuracy after hyperparameter tuning and ensembling.

# Conclusion
In this project, we explored various machine learning models to predict the popularity of online articles. The XGBoost algorithm stood out in both regression and classification tasks, delivering the best performance.

# References
- [Milestone 1 Report](./Milestone1 Report.pdf)
- [Milestone 2 Report](./Milestone2 Report.pdf)

