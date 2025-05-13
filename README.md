# Solar Flare Prediction Using Machine Learning

This project uses machine learning to predict **severe solar flares** based on space weather data.

## 🧠 What This Project Does

It looks at past solar activity (like sunspots and magnetic activity) and trains models to guess:
- Will there be a flare?
- If yes, will it be a strong one?

## 📁 Files in This Project

- `SolarFlareDataset.csv`: The data we used
- `solar_flare_model.ipynb`: The main notebook that runs everything
- `README.md`: This file
- `report.txt`: Summary of results

## 🧪 Models Used

We tried 3 machine learning models:
- Ridge Classifier
- K-Nearest Neighbors (KNN)
- Random Forest

We used a tool called **GridSearchCV** to help find the best settings for each model.

## 📊 Results

All three models were trained and tested. The best one is shown in the report with its accuracy.

## 🚀 How to Use

1. Open the notebook
2. Run each cell
3. Try entering your own solar data to get a prediction!

## 📌 Requirements

- Python
- scikit-learn
- pandas
- matplotlib
