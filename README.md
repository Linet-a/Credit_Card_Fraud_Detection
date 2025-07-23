# Fraud Detection with XGBoost

![Creditcard Fraud](https://media.licdn.com/dms/image/v2/C4E12AQGxNm7Bk_0iDQ/article-cover_image-shrink_720_1280/article-cover_image-shrink_720_1280/0/1630834609337?e=2147483647&v=beta&t=WSNr1rRZc4JV77escMP0MykuZibYY9BUCZkIzgO3WZA)

Credit card fraud is a significant and growing concern in the financial industry, leading to substantial financial losses and reduced customer trust. Fraudulent transactions are typically rare, making up a small fraction of all transactions, which creates a highly imbalanced classification problem.

The challenge lies in building a machine learning model that can accurately distinguish between fraudulent and non-fraudulent transactions using historical transaction data. The model must maximize detection of fraud (recall) while minimizing false positives, which can negatively affect customer experience and operational costs.

This project aims to develop a reliable fraud detection system using machine learning techniques, trained on a labeled dataset of credit card transactions. The goal is to empower financial institutions with an automated tool that flags suspicious transactions for further review or action.

### Data Understanding
The dataset used in this project contains credit card transaction data, where each row represents a single transaction. The key characteristics of the dataset are:

Total observations: 284,807 transactions

Fraudulent transactions: 492 (≈0.17%)

Non-fraudulent transactions: 284,315

Class imbalance: The dataset is highly imbalanced, with fraud cases being a very small fraction of the total.

📌 Features:
V1 to V28: Result of a PCA transformation to anonymize sensitive data like transaction time, amount, and customer information. These are numerical.

Time: Seconds elapsed between each transaction and the first transaction in the dataset.

Amount: The transaction amount.

Class: Target variable — 1 for fraud and 0 for non-fraud.

🔍 Key Insights from EDA:
Imbalance confirmed: Fraudulent transactions are rare.

No missing values: All features are complete.

Amount & Time needed scaling: Because they are on different scales than PCA features.

Outlier behavior: Fraudulent transactions often show distinct patterns in specific principal components.


### ⚙️ Features

- Manual resampling to balance training and validation sets.
-Logiststic Regression, Decision Tree,  XGBoost classifier, Deep Neural Network for modeling.
- ROC AUC curve and confusion matrix plotted for evaluation.
- Synthetic test data used to simulate model generalization.


### 🛠 Setup

1. Clone the repo:

   git clone https://github.com/Linet-a/Credit_Card_Fraud_Detection.git
   cd fraud-detection-xgboost


📁 Data

If you want to use the original dataset: https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud

Download from Kaggle Credit Card Fraud Dataset


🚧 To Improve
Enhance synthetic data generation to better mimic real fraud patterns

Try ensemble methods or anomaly detection techniques

Use techniques like SMOTE or ADASYN for more realistic oversampling

👤 Author
Linet Okinyi
