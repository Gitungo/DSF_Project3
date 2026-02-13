# DSF_Project3
DSF_Project3
## Customer Churn Prediction – Telecommunications Company
### Project Overview

Customer churn is a major challenge in the telecommunications industry. Acquiring new customers is significantly more expensive than retaining existing ones.

This project aims to:

Predict which customers are likely to churn

Identify key drivers of churn behavior

Support proactive retention strategies using machine learning

Two models were developed and compared:

Logistic Regression

Random Forest (including Balanced Random Forest)

### Business Objective

The primary goal is to:

Detect high-risk customers early

Reduce revenue loss

Enable targeted retention campaigns

Improve customer satisfaction through data-driven insights

### Dataset Description

The dataset contains customer behavioral and service usage information with the following features:

state

account length

international plan

voice mail plan

number vmail messages

total day minutes

total day calls

total day charge

total eve minutes

total eve calls

total eve charge

total night minutes

total night calls

total night charge

total intl minutes

total intl calls

total intl charge

customer service calls

churn (target variable)

The dataset is imbalanced, with a smaller proportion of customers churning.

### Exploratory Data Analysis (EDA)

Key insights identified:

Customers with more customer service calls show significantly higher churn rates.

International plan subscribers churn at higher rates.

High daytime usage correlates with churn.

Certain usage patterns and account characteristics increase churn likelihood.

Visualizations included:

Churn distribution

Churn rate by international plan

Churn rate by customer service calls

Usage comparisons

Feature importance analysis

### Modeling Approach
1. Logistic Regression

Baseline model

Linear decision boundary

Interpretable coefficients

2. Random Forest

Ensemble of decision trees

Captures nonlinear relationships

Handles complex feature interactions

Better suited for imbalanced behavioral data

### Model Evaluation Metrics

Due to class imbalance, accuracy was not sufficient.

The following metrics were used:

Precision – Accuracy of churn predictions

Recall – Ability to detect actual churners

F1 Score – Balance between precision and recall

AUC (ROC-AUC) – Overall separability of churners vs non-churners

### Model Performance Comparison
Metric	Logistic Regression	Random Forest
Precision	0.38	0.52
Recall	0.59	0.84
F1 Score	0.46	0.64
AUC	0.81	0.89
Key Findings:

Random Forest significantly outperformed Logistic Regression.

It detected 84% of churners.

It provided better overall class separation (AUC = 0.89).

It improved the balance between false positives and false negatives.

### Business Insights

Top drivers of churn:

High number of customer service calls

International plan subscription

High daytime usage

### Recommendations

Deploy the Random Forest model for churn prediction.

Adjust classification threshold based on business priorities.

Monitor performance regularly.

Integrate predictions into CRM systems for proactive retention actions.

Combine model predictions with customer service strategies.

### Technologies Used

Python

Pandas

NumPy

Scikit-learn

Imbalanced-learn

Matplotlib / Seaborn


### Conclusion

This project demonstrates how machine learning can be leveraged to:

Predict customer churn with high accuracy

Extract actionable business insights

Enable proactive, data-driven decision making

The Random Forest model provides a strong foundation for operational churn management.

