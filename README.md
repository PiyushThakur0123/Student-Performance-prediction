# Student Performance Prediction

A Data Science and Machine Learning project that analyzes behavioral, demographic, and academic factors to predict a student’s GPA and identify key drivers of academic success.

---

## Project Overview

This project explores student data to uncover actionable insights into what influences academic achievement. By leveraging **Mutual Information** for feature selection and training multiple regression models, the pipeline predicts a student's final **GPA** and categorizes their expected performance level.

---

## Key Features

* **Exploratory Data Analysis (EDA):** Visualizes feature correlation heatmaps and target GPA distributions.
* **Feature Importance:** Ranks variables (Study Time, Absences, Tutoring, Parental Support) using Mutual Information Regression.
* **Predictive Modeling:** Evaluates and compares three algorithms:
  * Linear Regression
  * Ridge Regression
  * Random Forest Regressor
* **Model Evaluation:** Benchmarks models using **MAE** and **$R^2$ Score**, supported by actual vs. predicted scatter plots.
* **Live Inference:** Accepts custom student inputs, scales features via `StandardScaler`, and forecasts performance (`Outstanding`, `Good`, `Improvement needed`).

---

## Tech Stack

* **Language:** Python
* **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-Learn

---

## Methodology

1. **Data Prep:** Cleaned features and removed non-predictive columns (`StudentID`, `GradeClass`).
2. **Analysis:** Calculated linear correlations and non-linear Mutual Information scores.
3. **Training:** Split data (80/20) and trained models using standardized scaling.
4. **Prediction:** Classified forecasted GPAs ($\ge 3.5$: *Outstanding*, $2.5 - 3.49$: *Good*, $< 2.5$: *Needs Improvement*).

---

