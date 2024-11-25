# Patient Treatment Recommendation System

### Overview

This repository contains a machine learning pipeline to recommend the most effective treatments for patients based on their profiles. The model leverages classification algorithms, similarity metrics, and feature engineering techniques to personalize recommendations, enabling data-driven clinical decision support.

### Objectives

Healthcare systems generate vast amounts of patient and treatment data. This project uses machine learning to:

- Predict treatment success based on patient profiles.
- Recommend the most suitable treatments for specific patients.
- Improve clinical outcomes by supporting data-driven decisions.

### Dataset

- Patient Data: Age, symptoms, chronic disease presence, and more.
- Treatment Data: Effectiveness and side-effect scores.
- Labels: Success or failure of treatments.

### Workflow

1. Data Preprocessing:
- Handles missing values with imputation.
- Encodes categorical variables.
- Normalizes numeric features.

2. Feature Engineering:
- Combines existing features to create derived metrics.
- Introduces patient-treatment similarity scoring.

3. Model Training:
- Logistic Regression, Random Forest, and XGBoost classifiers.
- GridSearchCV and RandomizedSearchCV for hyperparameter tuning.

4. Evaluation:
- Classification metrics (accuracy, precision, recall, F1-score).
- Recommendations evaluated using precision@k, recall@k, and NDCG@k.

5. Recommendations:
- Uses cosine similarity to suggest the most suitable treatments for each patient.

### Recommendation Evaluation

- Precision@2	1.000
- Recall@2	0.833
- NDCG@2	0.871

### Future Work

- Deep Learning: Experiment with neural networks for improved recommendations.
- Integration: Deploy as a web application or API for real-time recommendations.
- Bias Analysis: Audit the model for fairness across patient demographics.
- Explainability: Use SHAP or LIME to explain treatment predictions.

 ### Source

 https://www.kaggle.com/datasets/akashnath29/lung-cancer-dataset 
