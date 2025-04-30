# 🫀 Heart Attack Risk Prediction Dashboard

A full **Data Science mini-project** that explores the Heart Attack Risk Levels dataset through **EDA**, **visualizations**, and a **machine learning model** to predict a patient's risk level.

---

## 📊 Project Overview

This notebook-based project includes:

- ✅ Data cleaning and exploration with `pandas`
- 📈 Visualizations with `seaborn` and `matplotlib`
- 🧠 Predictive modeling using `RandomForestClassifier`
- 🔍 Feature analysis and correlation heatmaps
- 🎯 Target classification: `Low`, `Moderate`, `High` heart attack risk


## This project analyzes and models the **Heart Attack Risk Levels** dataset using Python, with a full data science workflow:

### 🔍 Step-by-Step Breakdown:

1. **Data Cleaning & Exploration**
   - Renamed columns for consistency
   - Checked data types, null values, and summary statistics
   - Visualized distributions of key risk factors (blood pressure, sugar, heart rate)

2. **Exploratory Data Analysis (EDA)**
   - Created histograms and KDE plots to understand feature behavior
   - Used a correlation heatmap to identify highly correlated risk indicators
   - Analyzed how risk levels vary across age, blood sugar, gender, etc.

3. **Data Preprocessing**
   - Encoded categorical labels (`Risk_Level`)
   - Scaled features with `StandardScaler`
   - Split data into training and testing sets (80/20)

4. **Model Building**
   - Trained a `RandomForestClassifier` on preprocessed data
   - Achieved **97.7% accuracy** on test set
   - Evaluated model using a classification report and confusion matrix

5. **Visualization of Results**
   - Plotted class distribution
   - Visualized confusion matrix
   - Illustrated blood sugar risk variation via histograms

---

✅ This project simulates a **real-world healthcare analytics task**, where early risk prediction can drive faster diagnosis and treatment.



---

## 🗂️ Dataset

- 📁 Source: [Kaggle – Heart Attack Risk Assessment](https://www.kaggle.com/datasets/fajobgiua/heart-attack-risk-assessment-dataset)
- 💡 Features:
  - Age, Gender, Heart Rate
  - Systolic & Diastolic Blood Pressure
  - Blood Sugar, CK-MB, Troponin
  - Risk Level Labels: `Low`, `Moderate`, `High`

---

## 📈 Model Results

The trained **Random Forest Classifier** showed excellent performance in predicting heart attack risk levels:

| Metric           | Value         |
|------------------|---------------|
| **Accuracy**     | 97.7%         |
| **Macro F1-Score** | 0.97        |
| **Classes**      | Low, Moderate, High |

### ✅ Class-wise Performance

| Risk Level | Precision | Recall | F1-Score |
|------------|-----------|--------|----------|
| **Low**    | 0.95      | 1.00   | 0.97     |
| **Moderate** | 1.00    | 0.93   | 0.97     |
| **High**   | 0.98      | 0.98   | 0.98     |

### 🔍 Confusion Matrix
![Confusion Matrix](./confusion_matrix.png)

These results indicate that the model:
- Accurately identifies **high-risk** individuals (critical for healthcare)
- Maintains strong balance across all classes
- Generalizes well to unseen data (no overfitting detected)

---

## 🧠 Key Takeaways

- **Blood Sugar** and **Troponin levels** show strong correlation with risk
- Minimal preprocessing was needed thanks to clean dataset
- Model performance is deployment-ready for clinical use cases



## 🚀 How to Run

### 📦 Step 1: Clone this repo
```bash
git clone https://github.com/your-username/heart-attack-risk-dashboard.git
cd heart-attack-risk-dashboard
