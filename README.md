# EV Charging Demand Predictor ⚡🚗

This project aims to build a machine learning-based model that predicts Electric Vehicle (EV) demand based on historical vehicle registration data. Accurate EV demand prediction is critical for planning and optimizing EV infrastructure such as charging stations, especially as the world shifts toward sustainable transportation.

---

## 🔍 Project Objective

To forecast the **Electric Vehicle (EV) Total** using relevant features like:
- Total Vehicles
- Non-Electric Vehicle Total
- Year
- County (encoded numerically)

This helps stakeholders such as government planners, city administrators, and private EV infrastructure providers to:
- Identify future demand hotspots
- Allocate resources efficiently
- Plan charging infrastructure based on real-world insights

---

## 🧠 How the Project Works

The project uses a dataset containing:
- County-wise vehicle registrations
- Total and non-electric vehicle counts
- Dates of registration

### Key Steps:
1. **Data Cleaning**: Removed commas, converted string numbers to numeric types, and extracted useful time features like year.
2. **Feature Engineering**: Encoded categorical data (e.g., counties) using `LabelEncoder`.
3. **Modeling**: Trained a machine learning regression model using **XGBoost**, a powerful gradient boosting algorithm.
4. **Evaluation**: Assessed the model using:
   - Mean Absolute Error (MAE)
   - R² Score
5. **Visualization**: Created graphs to understand trends, compare vehicle types, and visualize EV adoption patterns.

---

## 📊 Technologies & Libraries Used

- **Python**
- **pandas** – for data manipulation
- **matplotlib / seaborn** – for data visualization
- **scikit-learn** – for preprocessing & evaluation
- **XGBoost** – for model training and prediction

---

## 📁 Repository Structure

EV-Charging-Demand-Predictor/
│
├── week1/ # Data preprocessing and initial modeling
├── week2/ # Visualizations and model improvements
├── README.md # You're here!


---

## ✅ Outcomes

- A functional regression model that can predict EV demand based on vehicle trends.
- Enhanced interpretability using visual insights.
- Scalable approach that can be applied to other regions or extended with more features (e.g., population, fuel prices, policy data).

---
