🛰️ Solar Flare Prediction Using Machine Learning
This project uses machine learning to predict severe solar flares based on space weather data, helping anticipate risks to satellites, power grids, and communication networks.

🧠 What This Project Does
It analyzes past solar activity—such as sunspot classification, size, and distribution—to train models that predict:

Whether a solar flare will occur

If so, whether it will be severe

📁 Files in This Project
SolarFlareDataset.csv: Source dataset (NASA/NOAA format)

solar_flare_model.ipynb: Main notebook that trains and evaluates models

report.txt: Summary of findings

README.md: This file

⚙️ Preprocessing Highlights
Removed the rare class 2 (only 1 instance) to ensure balanced stratified sampling.

Used train_test_split(..., stratify=y, random_state=42) to maintain class distribution and ensure reproducibility.

Applied one-hot and ordinal encoding, along with standardization, in a ColumnTransformer pipeline.

🧪 Models & Evaluation
We tested three models using SMOTE to balance class labels and GridSearchCV for hyperparameter tuning:

Ridge Classifier

K-Nearest Neighbors (KNN)

Random Forest 🌟 (Best Performing)

We evaluated models using Precision, Recall, and F1-score (weighted average) to reflect balanced performance on an imbalanced dataset.

📊 Results (Weighted Avg)
Model	Precision	Recall	F1-score
Ridge	~0.96	~0.96	~0.96
KNN	~0.97	~0.97	~0.97
RandomForest	~0.98	~0.98	~0.98

🔧 Best parameters for each model are included in the output logs.

🌞 Why This Matters
Accurate prediction of severe solar flares is critical because:

NASA & Aerospace Missions: Can take precautions for crewed missions and sensitive instruments.

Utility Companies: Can protect power infrastructure from geomagnetic storms.

Telecoms & GPS Providers: Can anticipate and reduce signal disruption.

This model lays the foundation for real-time solar flare risk forecasting using Earth-based observations.

🚀 How to Use
Open solar_flare_model.ipynb

Run the cells in order

Input your own solar activity data to generate predictions

📌 Requirements
Python 3.8+

scikit-learn

pandas

matplotlib

seaborn

imbalanced-learn

