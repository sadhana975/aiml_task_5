# Heart Disease Prediction using Decision Tree & Random Forest

This project uses **Decision Tree** and **Random Forest** classifiers to predict the presence of heart disease from patient health data.

---

## Dataset
- File: `heart_disease.csv`  
- Contains **1025 records** and **14 features** including:
  - Age, Sex, Chest Pain (cp), Cholesterol (chol), Resting BP (trestbps), Fasting Blood Sugar (fbs), ECG results (restecg), Max Heart Rate (thalach), Exercise Angina (exang), ST Depression (oldpeak), Slope, Ca, Thal, and Target.  
- `target` column → `1` = Disease, `0` = No Disease.

---

##  Steps
1. Data Preprocessing:
   - Checked missing values, summary statistics, and dataset info.
   - Split into train/test sets (80/20).
2. Models Used:
   - **Decision Tree Classifier** (`max_depth=4`)
   - **Random Forest Classifier** (`n_estimators=100, max_depth=4`)
3. Evaluation:
   - Accuracy, Classification Report, Confusion Matrix
   - Feature Importances
   - Cross-validation (5-fold)

---

## Results
- **Decision Tree Accuracy**: ~85%  
- **Random Forest Accuracy**: ~90%  
- **Top Features**: Chest Pain (cp), Thal, Ca, Oldpeak

---

## Visualizations
- Confusion Matrix (Seaborn Heatmap)
- Decision Tree Plot (matplotlib & dtreeviz)
- Feature Importance Bar Graph

---

## How to Run
```bash
pip install -r requirements.txt
python heart_disease_model.py
Requirements
Python 3.x

scikit-learn

pandas, numpy

matplotlib, seaborn

graphviz, dtreeviz
