# Heart Stroke Prediction

## Project Overview
This project predicts the likelihood of a person having a stroke based on health-related parameters. It uses the Healthcare Dataset Stroke Data which includes demographic, medical, and lifestyle features.


## Dataset Information
- **Dataset Name:** `healthcare-dataset-stroke-data.csv`
- **Rows:** 5,110
- **Columns:** 12
- **Target Variable:** `stroke` (1 = Stroke, 0 = No Stroke)

### Features:
- `gender` – Male/Female/Other  
- `age` – Age of the person  
- `hypertension` – 0 (No), 1 (Yes)  
- `heart_disease` – 0 (No), 1 (Yes)  
- `ever_married` – Yes/No  
- `work_type` – Private, Self-employed, Govt_job, etc.  
- `Residence_type` – Urban/Rural  
- `avg_glucose_level` – Average glucose level  
- `bmi` – Body Mass Index  
- `smoking_status` – Smoking habits  

---

## Steps Performed
### 1. **Data Exploration**
- Checked dataset shape, info, descriptive stats
- Analyzed value counts for categorical features

### 2. **Data Visualization**
- **Line Plot** for `avg_glucose_level`
- **Histograms** for smoking status (stroke vs non-stroke)

### 3. **Data Cleaning & Preprocessing**
- Removed duplicates
- Handled missing values (`bmi` filled with 0)
- Converted `age`, `avg_glucose_level`, `bmi` to `int64`
- Normalized numeric features
- One-hot encoded categorical features

### 4. **Model Training**
- Train/Test Split: 70%-30%
- Applied:
  - **Logistic Regression** (classification)
  - **Linear Regression** (for comparison)

---

## Evaluation Metrics
### Logistic Regression:
- **Accuracy**
- **Precision, Recall, F1-score**

### Linear Regression:
- **Accuracy** (rounded predictions)
- **MSE**, **RMSE**, **MAE**, **R²**

---

## Results Summary
- **Logistic Regression** → Best for classification
- **Linear Regression** → Not ideal for classification tasks

---

## Technologies Used
- **Python**
- Libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`
