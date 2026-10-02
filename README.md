# EX-NO.-4a – MACHINE LEARNING MODEL – LINEAR REGRESSION

## AIM

To predict house prices using regression models and compare the performance of different machine learning regression models based on **RMSE, MAE, and R²**.

## INTRODUCTION TO MACHINE LEARNING

Machine Learning is used to learn patterns from existing data and make predictions.

* **Regression** is a supervised learning technique used to predict continuous numerical values.
* In this experiment, regression models are used to predict the **price of a house**.
* The dataset contains house-related features such as:

  * Square feet
  * Number of rooms
  * Age
  * Distance to city (km)

### Target Variable

* **Price**

---

# THEORY

## 1. Introduction

Linear Regression is a supervised machine learning algorithm used to predict a continuous numerical value based on one or more input variables.

It assumes that there is a linear relationship between the input variable(s) and the output variable.

For example, Linear Regression can be used to predict:

* House prices based on area
* Salary based on years of experience
* Sales based on advertising expenditure
* Temperature based on environmental factors
* Student marks based on study hours

## 2. Types of Linear Regression

### 2.1 Simple Linear Regression

Simple Linear Regression uses one independent variable to predict one dependent variable.

The equation is:

**y = b₀ + b₁x**

Where:

* **y** = Predicted output
* **x** = Input variable
* **b₀** = Intercept
* **b₁** = Slope/Coefficient

### 2.2 Multiple Linear Regression

Multiple Linear Regression uses two or more independent variables to predict the dependent variable.

The general equation is:

**y = b₀ + b₁x₁ + b₂x₂ + ... + bₙxₙ**

Where:

* **y** = Predicted output
* **b₀** = Intercept
* **b₁, b₂, ..., bₙ** = Regression coefficients
* **x₁, x₂, ..., xₙ** = Independent variables

---

# WORKING PRINCIPLE

The Linear Regression algorithm attempts to find the best-fit line through the available data points.

The best-fit line is selected by minimizing the difference between the actual values and the predicted values.

These differences are called **residuals or errors**.

The model commonly uses the **Least Squares Method**, which minimizes the sum of squared errors.

### Process Flow

```text
┌─────────────────────────────┐
│     House Price Dataset     │
└──────────────┬──────────────┘
               ↓
┌─────────────────────────────┐
│      Data Preprocessing     │
│ • Handle missing data       │
│ • Select features           │
│ • Scale data                │
└──────────────┬──────────────┘
               ↓
┌─────────────────────────────┐
│       Feature Selection     │
│ • Square Feet                │
│ • Number of Rooms            │
│ • Age                        │
│ • Distance to City (km)     │
└──────────────┬──────────────┘
               ↓
┌─────────────────────────────┐
│       Train-Test Split      │
└──────────────┬──────────────┘
               ↓
      ┌────────┴────────┐
      ↓                 ↓
┌───────────────┐ ┌────────────────┐
│ Regression    │ │ Regression     │
│ Model 1       │ │ Models 2, 3... │
└───────┬───────┘ └───────┬────────┘
        └─────────┬───────┘
                  ↓
┌─────────────────────────────┐
│     House Price Prediction  │
└──────────────┬──────────────┘
               ↓
┌─────────────────────────────┐
│      Model Evaluation       │
│ • RMSE                      │
│ • MAE                       │
│ • R²                        │
└──────────────┬──────────────┘
               ↓
┌─────────────────────────────┐
│ Compare Models and Select   │
│      the Best Model         │
└─────────────────────────────┘
```

---

# DATASET DESCRIPTION

* **Dataset:** House Price Dataset
* **Problem:** Predict house prices

### Features (X)

1. **square_feet** – Size of the house.
2. **num_rooms** – Number of rooms in the house.
3. **age** – Age of the house in years.
4. **distance_to_city (km)** – Distance from the city centre in kilometres.

### Target (y)

* **price** – Continuous house price.

---

# PROBLEM STATEMENT

* Develop a machine learning model to predict house prices.
* Use house characteristics as input variables.
* Train different regression models.
* Compare their prediction performance.
* Select the better-performing model based on evaluation metrics.

---

# REGRESSION MODELS USED

The notebook compares the following regression models:

1. **Linear Regression**
2. **Ridge Regression**
3. **Lasso Regression**
4. **ElasticNet Regression**
5. **Polynomial Regression**
6. **Decision Tree Regressor**
7. **Random Forest Regressor**
8. **Gradient Boosting Regressor**
9. **Support Vector Regressor (SVR)**
10. **K-Nearest Neighbors (KNN) Regressor**

---

# EVALUATION METRICS

The performance of the regression models is evaluated using the following metrics:

### 1. RMSE – Root Mean Squared Error

RMSE measures the average magnitude of prediction errors. A **lower RMSE** indicates better performance.

### 2. MAE – Mean Absolute Error

MAE measures the average absolute difference between actual and predicted values. A **lower MAE** indicates better performance.

### 3. R² – R-Squared

R² indicates how well the model explains the variation in the target variable. A **higher R²** generally indicates better performance.

---

# COLAB LINK

[Google Colab – EX-NO.-4a Machine Learning Model – Linear Regression](https://colab.research.google.com/drive/1Vszxt_Kk15eEIoMNZyvfMT2Ckvm5WY5s?utm_source=chatgpt.com)


---

# CONCLUSION

Thus, Linear Regression and other regression models were successfully applied for house price prediction. The performance of the different regression models was compared using standard evaluation metrics such as **RMSE, MAE, and R²**. Based on these metrics, the better-performing regression model can be selected for accurate house price prediction.
