# credit-risk-classification
Module 20 Challenge 
I was having trouble in step 1 of creating a logistic regression model. I used AI to help me over come the issue of the model not converging. Told me a fix was the set the iterations to 200. Seemed to have fixed the issue! I also used AI to help me build the layout of this README file.

# Loan Risk Prediction Analysis Report
## Overview of the Analysis
The purpose of this analysis is to build a machine learning model to predict whether a loan applicant is at high risk (default) or low risk (healthy loan). The goal is to assist the company in making data-driven lending decisions, reducing financial risk while ensuring eligible customers receive loans.

A logistic regression model was trained using historical loan data to classify loan statuses. The model's performance was evaluated using accuracy, precision, and recall to determine its reliability in real-world applications.

## Model Performance Metrics 
- Accuracy: 99% → The model correctly classifies 99% of loans as either high-risk or healthy.

- Precision:

  - Healthy Loans (0): 1.00 (Perfect—no misclassification)

  - High-Risk Loans (1): 0.84 (16% of predicted high-risk loans are actually healthy)

- Recall:

  - Healthy Loans (0): 0.99 (Only 1% of actual healthy loans are misclassified)

  - High-Risk Loans (1): 0.94 (6% of actual high-risk loans are missed)

## Summary of Results & Model Recommendation

Key Findings

Strengths:

- Extremely high accuracy (99%), meaning the model is very reliable for most cases.
  
- Strong recall (94%) for high-risk loans, ensuring that most actual defaults are correctly identified.
  
- Highly effective at predicting healthy loans with almost no errors.
  
⚠ Weaknesses:

- 16% false positive rate for high-risk loans, meaning some healthy loans are mistakenly classified as defaults.

- Class imbalance issue (18,765 healthy vs. 619 high-risk loans), which may bias the model toward predicting loans as low-risk.

## Recommendation: Should the Company Use This Model?

Not Recommended Without Adjustments

While the model performs very well overall, it may incorrectly deny too many good loans due to its false positive rate for high-risk loans. This could negatively impact customer satisfaction and business revenue.

Next Steps for Improvement

- Adjust the Decision Threshold to reduce false positives (lowering from 0.5 to 0.3).

- Explore Alternative Models (e.g., Random Forest, Gradient Boosting) to improve classification without sacrificing accuracy.

Final Verdict: The model has strong potential but should be refined before deployment to ensure fairer loan approvals while minimizing financial risk.
