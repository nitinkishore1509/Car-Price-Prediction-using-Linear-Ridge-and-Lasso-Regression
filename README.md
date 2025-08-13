# 🚗 Car Price Prediction using Linear, Ridge, and Lasso Regression

## 📌 Overview
This project focuses on predicting **car prices** using multiple regression techniques:
- **Linear Regression**
- **Ridge Regression**
- **Lasso Regression**

The aim is to build and compare models that can estimate the price of a car based on its features such as mileage, engine size, fuel type, horsepower, etc.  
We also explore **feature selection** and **regularization** to improve prediction accuracy and reduce overfitting.

---

## 🗂 Dataset
The dataset contains various attributes of cars including:
- **Car specifications** (e.g., make, model, fuel type, body style)
- **Performance metrics** (e.g., horsepower, engine size, mileage)
- **Market value** (target variable: price)

### Example Features:
| Feature         | Description |
|-----------------|-------------|
| make            | Car manufacturer |
| fuel-type       | Type of fuel used |
| horsepower      | Engine power |
| engine-size     | Size of engine in cubic inches |
| curb-weight     | Vehicle weight |
| price           | Target variable (car price in USD) |

---

## ⚙️ Methodology

### 1. **Data Preprocessing**
- Handling missing values
- Encoding categorical variables
- Scaling numerical features
- Splitting data into training and test sets

### 2. **Model Building**
- **Linear Regression**: Baseline model without regularization
- **Ridge Regression**: L2 regularization to prevent overfitting
- **Lasso Regression**: L1 regularization for feature selection

### 3. **Model Evaluation**
We used the following metrics to evaluate the models:
- **R² Score** (coefficient of determination)
- **Residual Sum of Squares (RSS)**
- **Mean Squared Error (MSE)**

---

## 📊 Results

| Metric            | Linear Regression | Ridge Regression | Lasso Regression |
|-------------------|-------------------|------------------|------------------|
| **R² Score (Train)** | 0.9757 | 0.9589 | 0.9465 |
| **R² Score (Test)**  | 0.8383 | 0.9224 | 0.9111 |
| **RSS (Train)**      | 2.10 × 10⁸ | 3.56 × 10⁸ | 4.63 × 10⁸ |
| **RSS (Test)**       | 7.02 × 10⁸ | 3.37 × 10⁸ | 3.86 × 10⁸ |
| **MSE (Train)**      | 1,213.00 | 1,577.72 | 1,799.94 |
| **MSE (Test)**       | 3,365.46 | 2,330.43 | 2,494.78 |

> **Key Insight:** Ridge regression achieved the highest **R² Score** on the test set, indicating better generalization compared to Linear and Lasso models. Lasso performed feature selection by shrinking less important coefficients to zero.

---

## 🖥️ Tech Stack
- **Python 3**
- **Libraries**:
  - pandas
  - numpy
  - matplotlib
  - seaborn
  - scikit-learn

---

