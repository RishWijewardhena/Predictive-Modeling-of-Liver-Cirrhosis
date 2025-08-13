# Liver Cirrhosis Prediction – Machine Learning Models

This project implements multiple machine learning models to predict liver cirrhosis patient outcomes based on clinical data.  
The workflow covers **data preprocessing**, **model training**, **hyperparameter tuning**, and **evaluation**.

---

## 📊 Dataset Preprocessing

- Removed duplicates and cleaned string columns.
- Converted categorical features into numerical form.
- Removed outliers using the **IQR method**.
- Normalized/standardized relevant numerical features.

---

## 🧠 Models Implemented

### 1. **XGBoost Classifier**
- Gradient boosting model optimized for structured tabular data.
- Tuned parameters with **Grid Search**.
- Key steps:
  ```python
  from xgboost import XGBClassifier
  model = XGBClassifier(eval_metric='mlogloss')
  model.fit(X_train, y_train)
