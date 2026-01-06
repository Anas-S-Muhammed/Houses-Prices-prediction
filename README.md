# Boston Housing Price Prediction

This repository contains my work on predicting house prices using the **Boston Housing Dataset**. The goal of this project is to explore data, visualize relationships, build machine learning models, and understand the end-to-end workflow of a machine learning project.

---

## Table of Contents

1. [Project Overview](#project-overview)  
2. [Dataset](#dataset)  
3. [Data Exploration & Visualization](#data-exploration--visualization)  
4. [Machine Learning Models](#machine-learning-models)  
   - Linear Regression  
   - Random Forest Regression  
5. [Evaluation](#evaluation)  
6. [Next Steps / Future Work](#next-steps--future-work)  
7. [Installation](#installation)  

---

## Project Overview

This project demonstrates:

- Loading and exploring the Boston Housing Dataset  
- Understanding feature correlations with house prices (`MEDV`)  
- Visualizing important features with **scatter plots** and **trend lines**  
- Building simple machine learning models:
  - Linear Regression  
  - Random Forest Regression  
- Evaluating models using **Mean Squared Error (MSE)** and **Root Mean Squared Error (RMSE)**  

---

## Dataset

The **Boston Housing Dataset** includes 506 houses with 13 features:

| Feature | Description |
|---------|-------------|
| CRIM | Crime rate by town |
| ZN | Proportion of residential land zoned for lots over 25,000 sq.ft. |
| INDUS | Proportion of non-retail business acres per town |
| CHAS | Charles River dummy variable (1 if tract bounds river; 0 otherwise) |
| NOX | Nitric oxides concentration |
| RM | Average number of rooms per dwelling |
| AGE | Proportion of owner-occupied units built prior to 1940 |
| DIS | Weighted distances to employment centers |
| RAD | Index of accessibility to radial highways |
| TAX | Full-value property-tax rate per $10,000 |
| PTRATIO | Pupil-teacher ratio by town |
| B | 1000(Bk - 0.63)^2 where Bk is the proportion of Black residents |
| LSTAT | % lower status population |
| MEDV | Median value of owner-occupied homes (target) |

---

## Data Exploration & Visualization

- Correlation analysis to find features most strongly associated with house prices:
  - `RM` → positive correlation with price  
  - `LSTAT` → strong negative correlation with price  
  - `PTRATIO` → moderate negative correlation  

- Scatter plots with trend lines were used to **visualize relationships**:
  - `% Lower Status vs Price`  
  - `Rooms vs Price`  
  - `Pupil-Teacher Ratio vs Price`  

---

## Machine Learning Models

### 1. Linear Regression

- Used `RM`, `LSTAT`, `PTRATIO` as input features  
- Trained and evaluated using `train_test_split`  
- Mean Squared Error (MSE) ≈ 27.11  
- Root Mean Squared Error (RMSE) ≈ 5.21 ($1000s)  

### 2. Random Forest Regression

- Used **all features** for prediction  
- Improved model performance compared to Linear Regression  
- Evaluated using MSE and RMSE  

---

## Evaluation

- Models were evaluated using:
  - **Mean Squared Error (MSE)**  
  - **Root Mean Squared Error (RMSE)**  
- Predictions were visualized against actual prices using scatter plots with a **perfect prediction line**.  

---

## Next Steps / Future Work

- Deploy the trained model using **Flask** or **Streamlit** as a web application  
- Hyperparameter tuning to improve Random Forest performance  
- Feature engineering to improve predictive accuracy  
- Try other ML algorithms such as Gradient Boosting or XGBoost  

---

## Installation

1. Clone the repository:

```bash
git clone https://github.com/YOUR_USERNAME/boston-housing-prediction.git
