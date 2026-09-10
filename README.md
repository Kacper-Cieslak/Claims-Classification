# Car Insurance Claim Prediction 🚗
## Overview

Binary classification project predicting whether a car insurance customer will make a claim.

Dataset: **10,000 observations, 18 features**  
Models compared: **Logistic Regression, KNN, Random Forest**

## Methodology
- preprocessing with `Pipeline` and `ColumnTransformer`
- Stratified 5-Fold Cross Validation
- hyperparameter tuning with `GridSearchCV`
- model selection based on **ROC-AUC**
- final evaluation on an untouched test set
- model interpretation with **Permutation Importance** and **Odds Ratios**

## Results
Best model: **Logistic Regression**

- CV ROC-AUC: **0.924**
- Test ROC-AUC: **0.916**
- PR-AUC: **0.832**
- Accuracy: **0.846**
- Precision: **0.758**
- Recall: **0.748**
- F1-score: **0.753**

The model generalized well to unseen data and correctly identified around **75% of actual claims**.

## Key Findings
`DRIVING_EXPERIENCE` was the strongest predictor of claim risk, followed by `POSTAL_CODE`, `VEHICLE_OWNERSHIP` and `VEHICLE_YEAR`.

The results show that a relatively simple and interpretable Logistic Regression model can achieve strong predictive performance without requiring a more complex model.

### Key illustrations
<img width="905" height="616" alt="image" src="https://github.com/user-attachments/assets/ba6fa1ea-11a1-4a96-89df-b5f2e24e8547" />
<img width="854" height="541" alt="image" src="https://github.com/user-attachments/assets/6dba9670-a94b-4640-a7fd-b6bcee5f68e0" />
