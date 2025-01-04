# House Price Prediction

This repository implements a linear regression model to predict house prices using the Boston Housing dataset. The project includes data preprocessing, feature scaling, and model training using gradient descent.

---

## Table of Contents

- [Introduction](#introduction)
- [Data Description](#data-description)
- [Techniques Used](#techniques-used)
- [Model Training](#model-training)
- [Evaluation Metrics](#evaluation-metrics)
- [How to Run](#how-to-run)
- [Requirements](#requirements)


---

## Introduction

This project implements a simple linear regression model to predict house prices using the Boston Housing dataset. The code includes data preprocessing, feature normalization, exploratory data analysis, and implementation of gradient descent for training the model.

---

## Data Description

The dataset provides information about housing prices based on various factors. It includes the following features:

- **CRIM**: Per capita crime rate by town.
- **ZN**: Proportion of residential land zoned for lots over 25,000 sq. ft.
- **INDUS**: Proportion of non-retail business acres per town.
- **CHAS**: Charles River dummy variable (1 if the tract bounds the river; 0 otherwise).
- **NOX**: Nitric oxide concentration (parts per 10 million).
- **RM**: Average number of rooms per dwelling.
- **AGE**: Proportion of owner-occupied units built prior to 1940.
- **DIS**: Weighted distances to five Boston employment centers.
- **RAD**: Index of accessibility to radial highways.
- **TAX**: Full-value property tax rate per $10,000.
- **PTRATIO**: Pupil-teacher ratio by town.
- **B**: 1000(Bk - 0.63)^2 where Bk is the proportion of Black residents by town.
- **LSTAT**: Percentage of lower-status population.
- **MEDV**: Median value of owner-occupied homes in $1000s (target variable).

---

## Techniques Used

- Data preprocessing (handling missing values, normalization)
- Feature scaling using Z-score normalization
- Implementation of linear regression from scratch
- Gradient descent optimization
- Visualization of relationships between features and the target variable

---

## Model Training

The model is trained using the following steps:
1. **Feature normalization**: All features are normalized using Z-score to ensure proper scaling.
2. **Gradient Descent**: The model parameters are optimized using gradient descent.
3. **Cost Function**: Mean squared error (MSE) is used as the cost function to evaluate the model's performance.

---

## Evaluation Metrics

The following metrics are used to evaluate the model:
- **Root Mean Squared Error (RMSE)**: Measures the average magnitude of errors.
---

## How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/your-repo-name.git
## **Requirements**

The following Python libraries are required to run the code:

- `numpy`
- `pandas`
- `matplotlib`
- `seaborn`

Install the dependencies using:

```bash
pip install numpy pandas matplotlib seaborn
