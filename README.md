# LoanTap - Loan Default Prediction (Logistic Regression)

## Overview

Analyzed LoanTap loan application data to understand borrower characteristics and identify factors associated with loan repayment risk. Developed a Logistic Regression classification model to predict loan outcomes and evaluate its ability to identify potentially risky borrowers using machine learning techniques.

## Dataset

The dataset contains borrower and loan-related information, including features such as:

* Loan amount
* Interest rate
* Annual income
* Employment length
* Home ownership
* Credit history
* Public record information
* Loan status (target variable)

The dataset was used to understand borrower profiles and build a predictive classification model.

## Objective

* Understand borrower characteristics and loan-related patterns
* Identify factors associated with loan repayment risk
* Perform data preprocessing and feature engineering
* Build a Logistic Regression classification model
* Evaluate model performance using classification metrics
* Generate business insights to support data-driven lending decisions

## Key Analysis

* Exploratory Data Analysis (EDA)
* Data Cleaning and Preprocessing
* Missing Value Treatment
* Categorical Feature Encoding
* Feature Scaling
* Feature Engineering (`has_pub_rec`)
* Train-Test Split with Stratification
* Handling Class Imbalance using Class Weights
* Logistic Regression Model Development
* Model Evaluation:
    * Accuracy
    * Precision
    * Recall
    * F1 Score
    * ROC-AUC
    * PR-AUC
* Confusion Matrix Analysis
* ROC Curve and Precision-Recall Curve
* Baseline Model Comparison

## Model Performance

The Logistic Regression model achieved the following results:

| Evaluation Metric | Score |
|---|---:|
| Accuracy | 64.45% |
| Precision | 31.14% |
| Recall | 67.09% |
| F1 Score | 42.54% |
| ROC-AUC | 0.7105 |
| PR-AUC | 0.3713 |

The model demonstrated improved minority-class identification compared with the baseline, particularly in terms of recall and F1 Score.

## Key Insights

* Class imbalance was an important challenge in the dataset.
* Class weighting helped improve the model's ability to identify the minority class.
* The model achieved a recall of approximately 67%, identifying a meaningful proportion of actual positive-class borrowers.
* The relatively low precision indicates that a considerable number of borrowers predicted as positive may not actually belong to the positive class.
* ROC-AUC of approximately 0.71 indicates that the model has a reasonable ability to distinguish between the two classes.
* The results highlight the importance of evaluating classification models using multiple metrics rather than relying only on accuracy.

## Model Interpretation (Business Understanding)

### Model Evaluation

The Logistic Regression model was evaluated using multiple classification metrics to understand its predictive performance.

* Recall measures the model's ability to identify actual positive-class borrowers.
* Precision measures the correctness of positive predictions.
* F1 Score provides a balance between precision and recall.
* ROC-AUC evaluates the model's ability to distinguish between the two classes.
* The confusion matrix helps identify false positives and false negatives.

### Business Interpretation

The model can support LoanTap in identifying potentially risky loan applicants by estimating the probability of belonging to the positive class.

However, the model's relatively low precision indicates that some borrowers may be incorrectly flagged as risky.

Further improvements through threshold optimization, feature selection, and comparison with other classification algorithms could help improve model performance and support more reliable lending decisions.

## Customer Risk Insights

* Borrower and loan characteristics can provide useful information for assessing repayment risk.
* Credit-related features may help identify patterns associated with loan outcomes.
* Class imbalance can affect the model's ability to identify risky borrowers.
* A classification threshold of 0.5 may not be optimal for every lending decision.
* The balance between identifying potential defaulters and avoiding incorrect risk classification is important for lending businesses.

## Tools Used

* Python
* Pandas, NumPy
* Matplotlib, Seaborn
* Scikit-learn
* Logistic Regression
* Classification Evaluation Metrics

## Business Impact

* Supports data-driven loan risk assessment
* Helps identify potentially risky borrowers
* Provides insights into borrower and loan characteristics
* Demonstrates the importance of class imbalance handling in financial classification problems
* Establishes a baseline machine learning model for further experimentation

By using machine learning to analyze borrower data, lending companies can improve risk assessment processes, make more informed lending decisions, and develop strategies to balance loan approval opportunities with default risk.
