# Week 3 - EV Charging Demand Predictor 🚗⚡

## 📌 Objective

In Week 3, we developed an **interactive web application** using **Streamlit** to showcase our EV Charging Demand Predictor. This app allows users to select a specific county and view predicted EV charging demand using pre-trained machine learning models.

---

## 🔧 Key Components

- **Streamlit App**: Simple, user-friendly interface to interact with the model.
- **Pre-trained Models**: RandomForestRegressor and DecisionTreeRegressor models are loaded using `joblib`.
- **Encoded County Selection**: `LabelEncoder` was used to convert county names into numeric codes required by the model.
- **Dynamic Graphs**: Interactive graphs display predicted vs actual demand trends.

---

## 🛠 Technologies Used

- Python
- Pandas, Scikit-learn, Matplotlib
- Streamlit
- Joblib (for loading ML models)

---

## ⚙️ How to Run the App

1. **Create a virtual environment (optional but recommended):**
   ```bash
   python -m venv venv
   venv\Scripts\activate    # for Windows
2. **Install dependencies:**
   ```bash
    pip install -r requirements.txt
3. **Run the Streamlit app:**
   ```bash
    streamlit run app.py

## 📈 Output Preview
Dropdown to choose county

Graphs showing:

Actual vs Predicted EV Charging Demand

Trends for each model

Insights into how different counties demand vary

## 💡 Improvements in Week 3
Integrated LabelEncoder to fix data format issues.

Improved user experience with clear visualization.

Addressed and fixed compatibility errors between model versions.

App now supports error-handling and works in isolated virtual environments.

## 📂 Files Included
app.py: Main Streamlit application.

preprocessed_ev_data.csv: Dataset with EV charging demand and county info.

RandomForest_model.pkl, DecisionTree_model.pkl: Trained ML models.

venv/: Virtual environment directory (not included in GitHub).
