Background and Overview
This project focuses on fraud detection using machine learning techniques. The objective is to develop models that can accurately identify fraudulent transactions within financial datasets. The problem is critical in industries such as banking and e-commerce, where timely detection of fraud can save significant financial losses. By leveraging a public dataset from Kaggle’s Bank Account Fraud Dataset Suite (NeurIPS 2022), this project applies multiple machine learning models, evaluates their performance using the AUC-ROC metric, and explores ensemble methods to boost detection accuracy.

Data Structure Overview
The dataset contains transactional data related to bank account activity, divided into labeled (fraud vs. non-fraud) and unlabeled categories. It is highly imbalanced, with fraud cases constituting a small percentage of the total records. Key features include:

Transaction ID: Unique identifier for each transaction.
Transaction Amount: Monetary value of the transaction.
Transaction Date/Time: Temporal details used for feature engineering.
Merchant Information: Categorical data on where the transaction occurred.
Fraud Label: Binary target variable (1 for fraud, 0 for non-fraud).
Executive Summary
The project explored four machine learning models: Logistic Regression, Random Forest, Neural Networks, and XGBoost. After hyperparameter tuning and model evaluation, the following results were achieved:

Logistic Regression AUC: 0.8719
Random Forest AUC: 0.8887
Neural Network AUC: 0.8793
XGBoost AUC: 0.8897
To further improve performance, an ensemble method using weighted averaging was implemented, resulting in an AUC of 0.8945, demonstrating a slight but meaningful improvement.

Insights Deep Dive
Imbalanced Data Handling: Since the dataset is highly imbalanced, techniques like oversampling and class weighting were applied to enhance model sensitivity to fraudulent cases.
Feature Engineering: Temporal features, such as transaction time of day, played a crucial role in distinguishing fraudulent activities.
Model Comparisons: XGBoost and Random Forest consistently outperformed Logistic Regression and Neural Networks, largely due to their ability to handle complex, non-linear relationships in the data.
Ensemble Strategy: The ensemble approach, particularly weighted averaging, proved effective in combining the strengths of different models, leading to higher AUC scores.
This project showcases the potential of machine learning for fraud detection, emphasizing the importance of data preprocessing, feature selection, and model selection in achieving robust results.
