### Fraud Detection with XGBoost

This project applies machine learning to detect fraudulent transactions. 


```
## ⚙️ Features

- Manual resampling to balance training and validation sets.
-Logiststic Regression, Decision Tree,  XGBoost classifier, Deep Neural Network for modeling.
- ROC AUC curve and confusion matrix plotted for evaluation.
- Synthetic test data used to simulate model generalization.

## 📊 Results

| Metric         | Value (Class 1 - Fraud) |
|----------------|--------------------------|
| Precision      | Low                      |
| Recall         | Low                      |
| Accuracy       | High (due to imbalance)  |
| ROC AUC        | Plotted below (see notebook) |

## 🛠 Setup

1. Clone the repo:
   ```bash
   git clone https://github.com/yourusername/fraud-detection-xgboost.git
   cd fraud-detection-xgboost
````




📁 Data
data/raw/: Original dataset (ignored by git)

data/processed/synthetic_test.csv: Synthetic test data to validate generalization

If you want to use the original dataset:

Download from Kaggle Credit Card Fraud Dataset

Place it in data/raw/

🚧 To Improve
Enhance synthetic data generation to better mimic real fraud patterns

Try ensemble methods or anomaly detection techniques

Use techniques like SMOTE or ADASYN for more realistic oversampling

👤 Author
Linet Okinyi