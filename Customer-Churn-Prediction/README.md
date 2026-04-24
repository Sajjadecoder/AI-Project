# Customer Churn Prediction

This project implements a machine learning pipeline to predict customer churn in a telecom dataset. The notebook `customer-churn-pred.ipynb` contains the complete analysis, from data exploration to model evaluation.

## Dataset

The dataset used is `data/telecom_churn.csv`, which contains telecom customer data with 3333 samples and 11 columns (10 features + 1 target variable: Churn). The features include:
- AccountWeeks: Number of weeks the customer has been with the company
- ContractRenewal: Whether the customer renewed the contract (1/0)
- DataPlan: Whether the customer has a data plan (1/0)
- DataUsage: Data usage in GB
- CustServCalls: Number of customer service calls
- DayMins: Daytime minutes used
- DayCalls: Number of daytime calls
- MonthlyCharge: Monthly charge
- OverageFee: Overage fee
- RoamMins: Roaming minutes
- Churn: Target variable (1 if churned, 0 otherwise)

## Pipeline Overview

### 1. Libraries Imports
- numpy
- pandas
- matplotlib.pyplot
- sklearn.model_selection.train_test_split

### 2. Exploratory Data Analysis (EDA)
- Dataset shape: (3333, 11)
- Data info: Column types and non-null counts
- Head of the dataset
- Null value check
- Churn distribution visualization (bar plot)

### 3. Preprocessing
- Feature-target split: X (features), y (Churn)
- Data splitting:
  - Train: 70% (2333 samples)
  - Validation: 15% (500 samples)
  - Test: 15% (500 samples)
- Standardization using StandardScaler
- Handling class imbalance with SMOTE (Synthetic Minority Over-sampling Technique) - balances the training set to have equal number of churn and non-churn samples

### 4. Model Training
Three models are trained:
- Logistic Regression (max_iter=1000)
- Decision Tree Classifier (random_state=42)
- Random Forest Classifier (random_state=42)

### 5. Evaluation on Validation Set
Models are evaluated using:
- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix

### 6. Model Comparison
Accuracy comparison bar plot:
- Logistic Regression: 79.4%
- Decision Tree: 86.0%
- Random Forest: 90.4%

### 7. Best Model Selection and Final Evaluation
Random Forest is selected as the best model(90.4% accuracy) and evaluated on the test set.

## Evaluation Results

### Validation Set Results

#### Logistic Regression
- Accuracy: 0.794
- Precision: 0.4268
- Recall: 0.8861
- F1 Score: 0.5761
- Confusion Matrix:
  [[327  94]
   [  9  70]]

#### Decision Tree
- Accuracy: 0.860
- Precision: 0.5495
- Recall: 0.6329
- F1 Score: 0.5882
- Confusion Matrix:
  [[380  41]
   [ 29  50]]

#### Random Forest
- Accuracy: 0.904
- Precision: 0.6867
- Recall: 0.7215
- F1 Score: 0.7037
- Confusion Matrix:
  [[395  26]
   [ 22  57]]

### Test Set Results (Random Forest)
- Accuracy: 0.928
- Precision: 0.7121
- Recall: 0.7344
- F1 Score: 0.7231
- Confusion Matrix:
  [[417  19]
   [ 17  47]]

## Dependencies

- numpy
- pandas
- matplotlib
- scikit-learn
- imbalanced-learn
- seaborn

Install via:
```
pip install -r requirements.txt
```

## How to Run

1. Ensure all dependencies are installed.
2. Open the notebook `customer-churn-pred.ipynb` in Jupyter.
3. Run all cells in order.
4. View the results and visualizations.

## Files

- `customer-churn-pred.ipynb`: Main notebook with the complete pipeline
- `data/telecom_churn.csv`: Dataset
- `requirements.txt`: Python dependencies
- `README.md`: This file