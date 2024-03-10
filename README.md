# Credit_Risk_Analysis
# Module 12 Report Template
___
## Overview of the Analysis

The primary goal of this analysis is to develop and assess machine learning models for predicting credit risk. By leveraging financial data related to loan applications, our objective is to construct models capable of effectively categorizing loans into either the healthy or high-risk categories. 
Two key iterations of the dataset were utilized for this analysis: the original dataset and a resampled version designed to mitigate class imbalance.

##Financial Information and Prediction Target:
The dataset includes various financial attributes related to loan applications. The predictive target is the loan status, with two distinct categories: healthy (0) and high-risk (1). The objective is to create models that can effectively classify loans into these two categories.

###Basic Information about Variables:
Loan Status (Target Variable):
Healthy (Class 0): 18,765 instances
High-Risk (Class 1): 619 instances

##Stages of the Machine Learning Process:
**1. Data Preprocessing:**

Exploratory Data Analysis (EDA) to understand data distributions and relationships.
Data cleaning and feature engineering to enhance model performance.

**2. Model Selection:**

Utilized the Logistic Regression algorithm due to its interpretability and suitability for binary classification tasks.

**3.Evaluation Metrics:**

Employed various metrics, including accuracy, precision, recall, and F1-score, to assess model performance.

**4.Resampling:**

Applied Random OverSampler to address class imbalance, specifically targeting the scarcity of high-risk loan instances.

##Methods Used

###Logistic Regression:

Chose this algorithm for its simplicity, interpretability, and effectiveness in binary classification tasks.
Resampling:

Utilized Random OverSampler to create a balanced representation of the minority class, improving the model's ability to identify high-risk loans.
This analysis follows a systematic approach, incorporating data preprocessing, model selection, evaluation metrics, and resampling to enhance the model's predictive capabilities, especially for the critical task of identifying high-risk loans. The methods employed aim to strike a balance between model interpretability and performance.

In summary, the choices made in model selection (Logistic Regression) and resampling method (Random OverSampling) were driven by the need for a transparent and interpretable model, coupled with the requirement to address class imbalance in the context of credit risk assessment. These decisions were made to achieve a balance between simplicity, interpretability, and effective model performance.



## Results

Machine Learning Model 1 (Logistic Regression - Original Data):

* Balanced Accuracy Score: 0.85
* Precision (High-Risk Loan - Class 1): 0.84
* Recall (High-Risk Loan - Class 1): 0.66
* F1-Score (High-Risk Loan - Class 1): 0.74


Machine Learning Model 2 (Logistic Regression - Resampled Data):


* Balanced Accuracy Score: 0.99
* Precision (High-Risk Loan - Class 1): 0.84
* Recall (High-Risk Loan - Class 1): 0.99
* F1-Score (High-Risk Loan - Class 1): 0.91

These scores provide a concise overview of the performance metrics for each machine learning model. The second model, trained with resampled data, shows superior results across all metrics, indicating enhanced accuracy and reliability in predicting high-risk loans.
## Summary

Summary of Machine Learning Model Results and Recommendation
Model Performance:
Logistic Regression Model (Original Data):
Balanced Accuracy Score: 0.85
Precision (High-Risk Loan - Class 1): 0.84
Recall (High-Risk Loan - Class 1): 0.66
F1-Score (High-Risk Loan - Class 1): 0.74
Logistic Regression Model (Resampled Data):
Balanced Accuracy Score: 0.99
Precision (High-Risk Loan - Class 1): 0.84
Recall (High-Risk Loan - Class 1): 0.99
F1-Score (High-Risk Loan - Class 1): 0.91
Recommendation:
The logistic regression model trained with resampled data outperforms the model trained on the original data. The resampled model demonstrates superior precision, recall, and F1-scores for high-risk loans, resulting in a significantly higher balanced accuracy score.
___
## Considerations
###Performance Comparison:

The resampled model achieves a balanced accuracy score of 0.99, indicating an excellent balance between sensitivity and specificity. This suggests superior performance in classifying both healthy and high-risk loans.

###Problem Dependence:

The nature of the credit risk prediction problem influences the choice of model. In this context, identifying high-risk loans (Class 1) is crucial. The resampled model excels in this regard, with high precision and recall for the high-risk class.
Importance of Predictions:

In credit risk assessment, correctly identifying high-risk loans is often more critical than predicting healthy loans. The resampled model's strong performance in predicting high-risk loans makes it more suitable for this specific problem.
Justification:
Given the task's emphasis on accurately identifying high-risk loans, the logistic regression model trained with resampled data is recommended. Its superior performance in precision, recall, and F1-score, along with the significantly higher balanced accuracy, positions it as the preferred model for making credit risk predictions. The resampling technique effectively mitigates class imbalance, enhancing the model's ability to identify and flag high-risk loan instances.





