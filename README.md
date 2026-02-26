# Fraud Detection: Tree-Based Models & Causal Study
**AC209A Course Project** *Authors: Krystal Qiu, Kaiyuan Huang, Jiangqi Wu, Gefei Shen*

## Project Goal
Developed a robust pipeline to identify fraudulent credit applications within a highly imbalanced dataset (~1.1% fraud rate). The project combines predictive power via ensemble methods with causal inference to understand behavioral risk factors.

## Key Features
* **Imbalanced Data Handling:** Utilized **SMOTE** and class-weight adjustments to manage extreme minority class rarity.
* **Structural Missingness:** Modeled informative missing values (e.g., address history) as distinct signals for fraud.
* **Predictive Modeling:** Implemented and tuned **XGBoost** and **Random Forest** classifiers, optimizing for **PR-AUC** and **Precision@50**.
* **Causal Inference:** Conducted a causal study on behavioral drivers—such as address stability and bank tenure—to move beyond correlation.

## Methodology
1. **Preprocessing:** Feature engineering, missing value imputation, and SMOTE oversampling.
2. **Modeling:** Comparative analysis between baseline Decision Trees and advanced Gradient Boosted Trees.
3. **Evaluation:** Focused on top-K ranking metrics relevant to financial operational goals.
4. **Causal Analysis:** Investigation of treatment effects for specific applicant behaviors.



## Tech Stack
* **Language:** Python
* **ML Libraries:** Scikit-learn, XGBoost, Imbalanced-learn
* **Data Analysis:** Pandas, NumPy, Matplotlib, Seaborn

## Results
The final models prioritize **Precision@50**, effectively identifying high-risk segments to reduce financial exposure while minimizing false positives for legitimate customers.
