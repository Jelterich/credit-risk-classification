# credit-risk-classification
Credit Risk Analysis Report
Overview of the Analysis
The purpose of this analysis is to predict the creditworthiness of borrowers using a logistic regression model. The dataset provided includes historical financial data for loans from a peer-to-peer lending company. Specifically:

Target Variable: loan_status
0: Healthy loan
1: High-risk loan
The goal was to train and evaluate a machine learning model that can effectively distinguish between healthy loans and high-risk loans to aid the company in better loan approval decisions.

The machine learning pipeline involved the following steps:

Data Preprocessing:
Separated the loan_status column as the target variable (y).
Created a features set (X) using all other columns.
Split the data into training (75%) and testing (25%) sets.
Model Training:
Trained a logistic regression model using the training data.
Model Evaluation:
Evaluated performance using a confusion matrix and classification report.
Results
The results of the logistic regression model are summarized below:

Accuracy: 99%

Precision:

0 (Healthy loan): 1.00
1 (High-risk loan): 0.84
Recall:

0 (Healthy loan): 0.99
1 (High-risk loan): 0.94
F1-Score:

0 (Healthy loan): 1.00
1 (High-risk loan): 0.89
These results demonstrate the model's ability to accurately classify loans while balancing precision and recall effectively for both categories.

Summary
The logistic regression model achieves exceptional performance:

The model has near-perfect accuracy (99%) and predicts healthy loans with 100% precision and 99% recall.
For high-risk loans, the model achieves 94% recall, meaning it successfully identifies the majority of actual high-risk loans. However, the precision is slightly lower at 84%, indicating some false positives (loans predicted as high-risk but are actually healthy).
Recommendation:
The model is highly effective and can be confidently recommended for credit risk classification.
Given the critical importance of identifying high-risk loans to minimize defaults, the high recall for 1 (94%) makes this model particularly valuable for the company.
Future improvements, such as balancing the dataset or exploring other algorithms (e.g., Random Forest or XGBoost), could further optimize precision without sacrificing recall