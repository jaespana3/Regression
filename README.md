# CHD Risk Prediction – Logistic Regression Project

## Overview

This project builds a logistic regression model to predict the 10-year risk of coronary heart disease (CHD) based on patient demographic, behavioral, and medical data. The model aims to support early risk identification and preventive care.

## Objective

* Predict the binary outcome: TenYearCHD (1 = CHD within 10 years, 0 = No CHD).
* Handle imbalanced data using `class_weight='balanced'`.
* Maximize recall and F1 score to detect at-risk individuals.
* Maintain interpretability for healthcare use.

## Dataset Description

Each row represents a patient. Key features include:

* **Demographic:** age, sex
* **Behavioral:** is\_smoking, cigsPerDay
* **Medical History:** prevalentHyp, diabetes, prevalentStroke, BPMeds
* **Current Health:** sysBP, diaBP, totChol, BMI, glucose, heartRate
* **Target:** TenYearCHD (0 or 1)

## Methodology

* Data cleaning: imputed missing values, clipped outliers.
* Feature selection based on domain knowledge.
* Standardized continuous variables.
* Used Logistic Regression with:

  * StandardScaler
  * `class_weight='balanced'`
* Evaluation with both default (0.5) and optimal threshold.
* Performance metrics include: Accuracy, Precision, Recall, F1 Score, ROC AUC.

## Files in this Repository

* `chd_logistic_regression.ipynb` — Jupyter notebook containing the complete analysis, including data preprocessing, model training, evaluation, and threshold selection.

## How to Use

1. Open `chd_logistic_regression.ipynb` in a Jupyter environment.
2. Follow the documented steps for data preprocessing, model fitting, and evaluation.
3. Review the classification metrics and threshold determination logic.
4. Adapt or extend the notebook for further exploration if desired.


