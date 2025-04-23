NAFLD-GenderML

This repository contains the source code and analysis for the article:

"Gender-Specific Machine Learning Models for Predicting NAFLD in Overweight Adults Using Clinical and Lifestyle Variables"

---

Project Overview

This research explores whether machine learning models trained separately on male and female datasets provide more accurate predictions of Non-Alcoholic Fatty Liver Disease (NAFLD) compared to models trained on combined data.

The dataset includes:
- Clinical variables (e.g., ALT, AST, FBS, Albumin, CHO)
- Anthropometric measures (BMI, BFP, WHR, Height, Weight)
- Lifestyle variables (Sleep Duration, Wake-Up Time)

---

Machine Learning Models Used

- Random Forest (RF)
- Support Vector Machine (SVM)
- Gradient Boosting (GB)
- K-Nearest Neighbors (KNN)

Each model was trained separately on:
- Male-only dataset
- Female-only dataset
- Combined dataset (general model)

---

Model Performance Summary

| Model | Dataset Type | Accuracy | AUC |
|-------|---------------|----------|-----|
| RF    | Male          | 0.75     | 0.7212 |
| SVM   | Female        | 0.60     | 0.5627 |
| SVM   | General       | 0.72     | 0.6994 |

These results suggest that **gender-specific models yield better predictive performance** for NAFLD classification.

---

SHAP Analysis (Explainability)

SHAP (SHapley Additive exPlanations) will be used to interpret the contribution of each feature across gender-specific models. This helps to identify which clinical or lifestyle features influence prediction differently for males and females.

Coming soon: SHAP summary plots and force plots.

---

Repository Contents

- `81new.ipynb` – Main notebook: preprocessing, training, evaluation
- `data_modified.csv` – Cleaned dataset
- `model_performance_summary.csv` – Accuracy, recall, precision, AUC tables
- `README.md` – Project description

---

Contact

Ali Estifa  
GitHub: [Nsport441](https://github.com/Nsport441)  
Email: estifa@gmail.com

---

> This code was developed as part of an academic research project in medical data science and is intended for research and educational use only.# NAFLD-GenderML
