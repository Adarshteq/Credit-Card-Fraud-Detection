## 🛡️ Credit Card Fraud Detection

A machine learning project to detect fraudulent credit card transactions using supervised learning algorithms. 

This project handles highly imbalanced data and uses multiple ensemble and deep learning techniques for fraud classification.

## 📁 Dataset

The dataset used is [creditcard.csv](./creditcard.csv), which contains transactions made by credit cards in September 2013 by European cardholders. 

It includes **284,807 transactions**, where **492 are frauds** (approx. 0.172%).

Features include:

- `Time`, `Amount` — raw input features

- `V1` to `V28` — result of a PCA transformation to protect user confidentiality

- `Class` — target variable (1 for fraud, 0 for non-fraud)

## 🧠 Models Used

Implemented in the [`Fraud_Detection.ipynb`](./Fraud_Detection.ipynb) notebook using:

- **Logistic Regression**

- **Random Forest**

- **XGBoost**

- **LightGBM**

- **CatBoost**

- **Neural Networks (TensorFlow/Keras)**

Handling of class imbalance was achieved using **SMOTE** and other techniques from `imbalanced-learn`.

## 📊 Evaluation Metrics

Due to the class imbalance, traditional accuracy isn't sufficient. We focus on:

- Precision

- Recall

- F1-Score

- ROC-AUC

- Confusion Matrix

- PR Curve

## 🧰 Requirements

Install all dependencies via:

```bash
pip install -r requirements.txt
````

Main libraries used:

* `numpy`, `pandas`
* `matplotlib`, `seaborn`
* `scikit-learn`
* `xgboost`, `lightgbm`, `catboost`
* `imbalanced-learn`
* `tensorflow`

For full details, check [`requirements.txt`](./requirements.txt).

## 🚀 Getting Started

1. Clone this repository:

   ```bash
   git clone https://github.com/your-username/credit-card-fraud-detection.git
   cd credit-card-fraud-detection
   ```

2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Launch the Jupyter notebook:

   ```bash
   jupyter notebook Fraud_Detection.ipynb
   ```
