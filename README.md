# 🚦 Traffic Demand Prediction using CatBoost

## 📌 Overview

This project was developed for **Gridlock Hackathon 2.0**. The objective was to predict urban traffic demand using historical road and environmental data.

A machine learning pipeline was built using **CatBoost Regressor**, which efficiently handles categorical features and missing values.

---

## 📂 Dataset Features

- Geohash (Location)
- Day
- Timestamp
- Road Type
- Number of Lanes
- Large Vehicles
- Landmarks
- Temperature
- Weather

**Target Variable**

- `demand`

---

## ⚙️ Data Preprocessing

- Loaded separate training and testing datasets.
- Handled missing numerical values using median imputation.
- Replaced missing categorical values with `"Unknown"`.
- Prepared categorical features for CatBoost.

---

## 🛠️ Feature Engineering

The following features were extracted from the timestamp column:

- Hour
- Minute
- Rush Hour Indicator
- Weekend Indicator

---

## 🤖 Model

**Algorithm:** CatBoost Regressor

| Hyperparameter | Value |
|---------------|--------|
| Iterations | 1500 |
| Learning Rate | 0.05 |
| Depth | 8 |
| Loss Function | RMSE |

---

## 📊 Results

| Metric | Score |
|----------|----------|
| Local Validation R² | **94.19%** |
| Public Leaderboard Score | **90.273** |

---

## 🧰 Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- CatBoost
- Jupyter Notebook
- Google Colab

---

## 📁 Project Structure

```text
Traffic-Demand-Prediction-CatBoost/
│
├── traffic_prediction.ipynb
├── train.csv
├── test.csv
├── sample_submission.csv
├── submission.csv
└── README.md
```

---

## 🚀 Future Improvements

- Time-aware cross validation
- Hyperparameter optimization
- Ensemble learning (CatBoost + XGBoost)
- Advanced feature engineering
- Model deployment using FastAPI and Docker

---

## 🏆 Competition

**Gridlock Hackathon 2.0**

This project was developed as part of the hackathon challenge to explore machine learning techniques for intelligent urban traffic prediction.
