# 🌾 Crop Yield Prediction using Machine Learning

## Overview

This project implements an end-to-end **machine learning regression model** to predict crop yield using real-world agricultural and environmental data. The solution focuses on **data preprocessing, model selection, evaluation, and reasoning**, as required for an AI/ML Engineer role.

This project was developed as part of a **campus recruitment assignment**.

---

## Problem Statement

Build a predictive machine learning model using a real or public dataset that can estimate a future value and explain the results.

---

## Dataset

* Source: Public Kaggle Crop Yield Dataset
* Type: Real-world agricultural data
* Records: ~28,000

### Features Used

* Area (Region)
* Item (Crop Type)
* Year
* Average Rainfall
* Average Temperature
* Pesticide Usage

### Target Variable

* Crop Yield (hg/ha)

---

## Machine Learning Pipeline

```
Data Loading
   ↓
Data Cleaning & Preprocessing
   ↓
Categorical Encoding
   ↓
Feature Selection
   ↓
Train–Test Split
   ↓
Baseline Model (Linear Regression)
   ↓
Improved Model (Random Forest Regressor)
   ↓
Evaluation (MAE, RMSE, R²)
   ↓
Inference
```

---

## Data Preprocessing

* Removed unnecessary columns
* Checked and handled missing values
* Encoded categorical variables (`Area`, `Item`) using Label Encoding
* Selected relevant environmental and agricultural features

---

## Models Implemented

### 1. Linear Regression (Baseline)

* Used to establish a basic reference model
* Limited performance due to linear assumptions

### 2. Random Forest Regressor (Final Model)

* Captures non-linear relationships in data
* Significantly improved performance over baseline

---

## Evaluation Metrics

This is a **regression problem**, so the following metrics were used:

* Mean Absolute Error (MAE)
* Root Mean Squared Error (RMSE)
* R² Score

### Final Model Performance (Random Forest)

* **MAE:** ~3,700
* **RMSE:** ~10,000
* **R² Score:** ~0.98

The high R² score indicates strong predictive capability on real-world data.

---

## Inference

The trained model can predict crop yield for new input conditions such as:

* Crop type
* Region
* Year
* Rainfall
* Temperature
* Pesticide usage

This demonstrates the model’s ability to generalize to unseen data.

---

## Project Structure

```
Crop-Yield-Prediction/
│
├── crop_yield_prediction.ipynb   # Complete ML implementation
├── yield_df.csv                  # Dataset
├── README.md                     # Project documentation
└── requirements.txt              # Dependencies
```

---

## How to Run

1. Install dependencies:

```bash
pip install -r requirements.txt
```

2. Open the notebook:

```bash
jupyter notebook crop_yield_prediction.ipynb
```

(or run in Google Colab)

3. Execute all cells to perform preprocessing, training, evaluation, and inference.

---

## Key Takeaways

* Demonstrates strong **ML fundamentals**
* Handles real-world data preprocessing challenges
* Compares baseline and improved models
* Focuses on **model reasoning**, not just accuracy
* Fully aligns with AI/ML Engineer evaluation criteria

---

## Author

**Kakumanu Pujitha**

---

