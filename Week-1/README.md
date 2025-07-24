# Week 1: Data Preprocessing & Initial Modeling

This folder contains the Week 1 work for the **EV Charging Demand Predictor** project. The main focus during this phase was on **data cleaning, transformation, feature engineering**, and building the **initial regression model** to predict EV demand.

---

## 📌 Objectives for Week 1

- Load and explore the dataset
- Clean and preprocess the data
- Convert object types to numeric
- Encode categorical variables (e.g., County)
- Train a basic regression model using XGBoost

---

## 🛠️ Key Tasks Completed

### 🔹 1. Data Cleaning

- Removed commas from values like `'3,382'` using `.str.replace(',', '')`
- Converted columns like `Total Vehicles` and `Non-Electric Vehicle Total` to numeric types

### 🔹 2. Feature Engineering

- Extracted the **Year** from the `Date` column
- Encoded the `County` column using `LabelEncoder` to prepare it for modeling:
  
  ```python
  from sklearn.preprocessing import LabelEncoder
  le = LabelEncoder()
  df['county_encoded'] = le.fit_transform(df['County'])
