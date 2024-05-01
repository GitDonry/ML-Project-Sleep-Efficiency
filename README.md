# ML-Project-Sleep-Efficiency
The focus will be on linear regression and its regularized variants, namely Lasso and Ridge Regression. And use random forest as a comparative model.

1. Problem
Sleep quality is an essential factor in human health and well-being. Many individuals suffer from sleep disorders or low sleep efficiency, impacting their daily functioning, mental health, and overall physical wellness. The primary objective of this project is to develop a regression model that accurately predicts sleep efficiency, measured as a continuous variable, based on various factors. 
 
2. Data
Description: The dataset, "Sleep_Efficiency.csv," contains individual-specific sleep-related data. It includes various attributes that potentially influence sleep efficiency. 
Dimensions: 452 entries, each with 15 features.
Features:
Numeric: Age, Sleep Duration, REM Sleep Percentage, Deep Sleep Percentage, Light Sleep Percentage, Awakenings, Caffeine Consumption, Alcohol Consumption, Exercise Frequency.
Categorical: Gender, Smoking Status.
Temporal: Bedtime, Wakeup Time.
Source: The dataset is obtained from Kaggle, ensuring diverse and unbiased data for analysis. Citation: https://www.kaggle.com/datasets/equilibriumm/sleep-efficiency
 
3. Approach
The focus will be on linear regression and its regularized variants, namely Lasso and Ridge Regression. And use random forest as a comparative model.
Models:
Linear Regression: Serves as a baseline model, offering simplicity and interpretability.
Lasso Regression:  Introduces feature selection and regularization to handle overfitting.
Ridge Regression: Addresses multicollinearity effectively.
Random Forest: An ensemble model to compare against linear models.
Why exclude other approaches:
Logistic Regression: Unsuitable due to the continuous response variable.
KNN: Less interpretable, computationally intensive for straightforward linear relationships.
Decision Tree: Can be overly complex and less interpretable than linear regression.
Bagging and Boosting: Require more resources and training time, making hyperparameter selection difficult.
Data Preprocessing:
Managing missing values through imputation or removal.
Standardizing numerical data to ensure consistent scale.
Encoding categorical variables for regression analysis.
Feature Selection: 
VIF: VIF to check for multicollinearity.
BIC: We used subset selection, followed by BIC comparison to identify the optimal model to ensure a robust model with a balanced predictor set.
Hyperparameter Tuning:
Determining the optimal regularization strength (lambda) for Lasso and Ridge Regression by evaluating performance (RMSE) through 10-fold cross-validation. The best lambdas we found are both 0.01.
