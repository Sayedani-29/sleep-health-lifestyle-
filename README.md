# 😴 Sleep Health & Lifestyle — Sleep Disorder Prediction

A machine learning project that analyzes sleep health and lifestyle data to predict sleep disorders (Insomnia, Sleep Apnea, or None) using multiple classification models.

## 📌 Overview

This project performs end-to-end data analysis and classification on a sleep health dataset. It includes exploratory data analysis (EDA), preprocessing, and training of three classification models — Logistic Regression, Decision Tree, and Random Forest — with hyperparameter tuning via GridSearchCV.

## 📂 Dataset

- **File:** `Sleep_health_and_lifestyle_dataset.csv`
- **Target Variable:** `Sleep Disorder` (No Disorder / Insomnia / Sleep Apnea)
- **Features:** Age, Gender, Occupation, Sleep Duration, Quality of Sleep, Physical Activity Level, Stress Level, BMI Category, Blood Pressure, Heart Rate, Daily Steps

## 🔍 Project Workflow

1. **Data Loading & Cleaning** — Handling nulls, splitting Blood Pressure into Upper/Lower BP, dropping irrelevant columns
2. **EDA** — Distribution plots, pair plots, count plots, box plots, pie charts by gender, occupation, BMI, stress level, and sleep quality
3. **Key Observations:**
   - Nurses are most affected by Sleep Apnea
   - Salespersons have the highest rate of Insomnia
   - Overweight individuals have higher chances of sleep disorder
   - Sleep Apnea is more common in females; Insomnia is more common in males
4. **Preprocessing** — Label Encoding for categorical variables, correlation heatmap analysis
5. **Model Training & Evaluation** — Accuracy, F1 Score, Precision, Recall, Jaccard Score, Confusion Matrix

## 📊 Models Used

| Model | Accuracy | F1 Score |
|-------|----------|----------|
| Logistic Regression | 67.26% | 0.67 |
| Decision Tree (tuned) | 90.27% | 0.9 |
| Random Forest (tuned) | 89.37% | 0.87 |

## 🛠️ Tech Stack

- Python, Pandas, NumPy
- Scikit-learn (LabelEncoder, GridSearchCV, classifiers)
- Matplotlib, Seaborn, Plotly
- Jupyter Notebook / Google Colab

## 🚀 How to Run

```bash
git clone https://github.com/yourusername/sleep-health-lifestyle
cd sleep-health-lifestyle
pip install -r requirements.txt
jupyter notebook sleep_health_lifestyle.ipynb
```

> **Note:** Update the dataset path in the notebook if not using Google Drive.

## 📄 License
MIT
