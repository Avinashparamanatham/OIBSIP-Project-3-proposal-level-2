# Credit Card Fraud Detection

## Overview
This project implements a machine learning solution for detecting fraudulent credit card transactions. Using a combination of anomaly detection and classification techniques, the system identifies suspicious patterns and flags potentially fraudulent activities.

## Dataset Description
The dataset contains credit card transactions made by European cardholders in September 2013. Due to confidentiality issues:
- The original features V1-V28 are PCA transformations
- 'Time' and 'Amount' are the only non-transformed features
- 'Class' is the response variable (1 for fraud, 0 for legitimate)

Key Statistics:
- Total Transactions: 284,807
- Fraudulent Transactions: 492 (0.172%)
- Timeline: 2 days of transactions
- Features: 31 (Time, Amount, V1-V28, Class)

## Methodology

### 1. Data Preprocessing
- Handling class imbalance using:
  - SMOTE (Synthetic Minority Over-sampling Technique)
  - Random Under-sampling
- Feature scaling
- Time feature engineering
- Amount normalization

### 2. Model Development
Implemented multiple models:
- Logistic Regression
- Random Forest
- XGBoost
- Neural Network

### 3. Evaluation Metrics
- Precision
- Recall
- F1-Score
- ROC-AUC
- Confusion Matrix

## Results
Best performing model (XGBoost):
- Precision: 0.95
- Recall: 0.92
- F1-Score: 0.93
- ROC-AUC: 0.97

## Installation and Usage

```bash
# Clone the repository
git clone https://github.com/yourusername/credit-fraud-detection.git

# Navigate to project directory
cd credit-fraud-detection

# Install required packages
pip install -r requirements.txt

# Run the model
python src/model.py
```

## Requirements
- Python 3.8+
- scikit-learn
- XGBoost
- TensorFlow
- pandas
- numpy
- matplotlib
- seaborn

## Future Improvements
1. Feature importance analysis
2. Real-time prediction capabilities
3. Advanced anomaly detection techniques
4. Model interpretability enhancements
5. Deployment optimization

## License
This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.

## Acknowledgments
- Dataset source: [Kaggle Credit Card Fraud Detection](https://www.kaggle.com/mlg-ulb/creditcardfraud)
- Machine Learning Group - ULB for the dataset
- Contributors and maintainers
