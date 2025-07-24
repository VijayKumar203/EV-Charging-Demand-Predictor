
---

### ✅ 2. **Week 1 `README.md`**  
📁 Path: `/week1/README.md`

```markdown
# Week 1: Data Preprocessing & Initial Model Development 🧪

## ✅ Tasks Completed

- Loaded the dataset and explored key columns like `Date`, `County`, `Total Vehicles`, `Electric Vehicle (EV) Total`, and `Non-Electric Vehicle Total`.
- Converted `Date` into datetime format and extracted the year.
- Handled data type issues (e.g., converting string values with commas into integers).
- Added `county_encoded` column using `LabelEncoder` to prepare the data for modeling.
- Performed initial train-test split and used `XGBRegressor` for model training.
- Evaluated performance using MAE and R² score.

## 🔍 Key Code Additions

```python
from sklearn.preprocessing import LabelEncoder
le = LabelEncoder()
df['county_encoded'] = le.fit_transform(df['County'])
