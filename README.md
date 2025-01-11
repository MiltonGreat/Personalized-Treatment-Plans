# Patient Treatment Recommendation System

### Overview: 

This project addresses the challenge of personalized clinical decision-making by developing a machine learning-based system to recommend the most effective treatments for patients. Leveraging classification algorithms and similarity metrics, the system achieved 87% accuracy, enhancing treatment efficacy and supporting data-driven healthcare decisions.

### Problem Statement

Problem: Clinical decision-making often requires processing complex and large-scale patient data to recommend treatments. However, many existing systems lack personalization, leading to suboptimal outcomes.

Significance: By leveraging machine learning, this project aims to provide tailored treatment recommendations, improving clinical outcomes and optimizing healthcare efficiency.

### Data

- Patient Medical Records: Age, symptoms, chronic diseases, and other health indicators.
- Treatment Data: Effectiveness ratings and side-effect scores.
- Labels: Success or failure of treatments.

### Solution Approach:

1. Data Cleaning
- Missing Data: Numerical features were imputed using median values, and categorical features were imputed using mode.
- Normalization: Applied Min-Max scaling to normalize numeric features.

2. Exploratory Data Analysis (EDA)
- Identified key correlations between patient attributes and treatment success.
- Visualized data distributions to uncover patterns and potential biases.

3. Feature Engineering
- Created derived metrics highlighting critical health indicators.
- Introduced patient-treatment similarity scores using cosine similarity.

4. Model Building
- Algorithms: Tested Logistic Regression, Random Forest, and XGBoost.
- Optimization: Hyperparameters were fine-tuned using GridSearchCV and RandomizedSearchCV.

5. Evaluation
- Used metrics including accuracy, precision, recall, F1-score, and ROC-AUC.
- Evaluated treatment recommendations with precision@k, recall@k, and NDCG@k.

### Results: 

- Model Performance: Achieved 87% accuracy in predicting treatment success.
- Precision@2: 1.000
- Recall@2: 0.833
- NDCG@2: 0.871

### Challenges: 

- Imbalanced Data: Mitigated using SMOTE to balance class distributions.
- Missing Data: Addressed using imputation techniques for robust predictions

### Future Work

- Deep Learning: Experiment with neural networks for improved recommendations.
- Integration: Deploy as a web application or API for real-time recommendations.
- Bias Analysis: Audit the model for fairness across patient demographics.
- Explainability: Use SHAP or LIME to explain treatment predictions.

 ### Source

 https://www.kaggle.com/datasets/akashnath29/lung-cancer-dataset 
