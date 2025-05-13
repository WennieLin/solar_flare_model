# 🌞 Solar Flare Prediction using Machine Learning

This project focuses on predicting **severe solar flares** based on solar activity data using classification models. The dataset includes solar sunspot features such as Zurich classification, spot size, distribution, and other observed characteristics.

---

## 📁 Dataset

- **Source**: `SolarFlareDataset.csv`
- **Target Variable**: `severe flares` (binary: 0 = no severe flare, 1 = severe flare)
- **Features**:
  - `modified Zurich class` *(ordinal)*
  - `largest spot size` *(ordinal)*
  - `spot distribution` *(nominal)*
  - `activity`, `evolution`, `area`, etc. *(numerical)*

---

## 🧠 Models Used

- **Ridge Classifier**
- **K-Nearest Neighbors (KNN)**

---

## ✅ Tasks Completed

| Task                                                                 | Status  |
|----------------------------------------------------------------------|---------|
| Proper encoding of categorical features (ordinal vs. nominal)        | ✅ Done |
| Train/test split of the dataset                                      | ✅ Done |
| Hyperparameter tuning via `GridSearchCV`                             | ✅ Done |
| Classification performance evaluation (precision, recall, F1-score) | ✅ Done |
| Visualization of key feature relationships                          | ✅ Done |

---

## 📊 Visualizations

- **Correlation Heatmap** of numerical features vs `severe flares`
- **Bar Chart** showing average severe flare rate by `modified Zurich class`

---

## 🔍 Key Insights

- Ridge and KNN models both achieved strong weighted F1-scores.
- Severe flares are rare, making this an imbalanced classification problem.
- Zurich classes like `F` and `H` show higher association with severe flares.

---

## 🚀 Future Work

- Introduce **more models** (e.g., XGBoost, GradientBoosting)
- Use **SMOTE** or class weighting for class imbalance
- Engineer **temporal features** (if time data is available)
- Perform **feature selection** or dimensionality reduction

---

## 🛠 How to Run

1. Upload `SolarFlareDataset.csv`
2. Run `solar_flare_model_revised.ipynb` in Google Colab or Jupyter
3. Review model results and visualizations

---

## 📧 Author

Wennie Lin  
Capstone Project – Solar Flare Prediction  
May 2025  
