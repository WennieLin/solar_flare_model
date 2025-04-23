# 🌞 Solar Flare Regression Project (with Log Transformation)

This project performs **exploratory data analysis (EDA)** and builds **machine learning regression models** to predict solar flare intensity using the NASA Solar Flare Dataset. We apply a **logarithmic transformation** to handle skewness in the target variable.

## 📁 Dataset Overview

- **Records**: 1,389 solar observations
- **Features**: 13 (categorical + numerical)
- **Final Target**: `log(total_flares)` where `total_flares = moderate + severe flares`

## 🔍 Objectives

1. Understand solar flare data distributions
2. Clean and encode categorical features
3. Build baseline and advanced ML models
4. Apply log transformation to improve prediction accuracy
5. Interpret feature importance

## 🛠️ Feature Engineering

- **Label Encoding** for:
  - `modified Zurich class`
  - `largest spot size`
  - `spot distribution`
- **New Target**: 
  - `total_flares = moderate flares + severe flares`
  - Transformed to: `log_total_flares = log1p(total_flares)`

## ⚙️ Modeling

| Model                     | MAE   | RMSE  | MSE   |
|---------------------------|-------|-------|-------|
| Random Forest (original) | 0.145 | 0.374 | 0.140 |
| ✅ Random Forest (log)   | 0.113 | 0.316 | 0.100 |

> Log transformation improved prediction accuracy and reduced error on original scale.

## 🔥 Feature Importance

Most influential features:
- `evolution`
- `previous 24 hour flare activity`
- `historically-complex`
- `area`
- `activity`
