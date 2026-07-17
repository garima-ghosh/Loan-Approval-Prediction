# Loan Approval Prediction using Machine Learning

## Project Overview

This project predicts whether a loan application will be **Approved** or **Rejected** using Machine Learning classification algorithms.

The project includes data preprocessing, feature engineering, model training, model evaluation, and model comparison to select the best-performing algorithm.

---

## Objective

To build a machine learning model that predicts loan approval based on an applicant's financial and personal information.

---

## Dataset

The dataset contains information about loan applicants.

### Features

- Number of Dependents
- Education
- Self Employed
- Annual Income
- Loan Amount
- Loan Term
- CIBIL Score
- Residential Assets
- Commercial Assets
- Luxury Assets
- Bank Assets

### Target Variable

- Loan Status
  - Approved
  - Rejected

---

## Data Preprocessing

The following preprocessing steps were performed:

- Removed unnecessary spaces from column names
- Created a new feature:
  - Total Assets = Residential + Commercial + Luxury + Bank Assets
- Converted categorical variables using Label Encoding
- Split the dataset into Training and Testing sets
- Applied Standard Scaling for Logistic Regression

---

## Machine Learning Models

The following models were trained and compared:

- Logistic Regression
- Decision Tree
- Random Forest

---

## Model Evaluation Metrics

The models were evaluated using:

- Accuracy
- Confusion Matrix
- Precision
- Recall
- F1 Score
- ROC-AUC Score
- 5-Fold Cross Validation

---

## Results

| Model | Accuracy |
|--------|---------:|
| Logistic Regression | 92.15% |
| Decision Tree | 98.13% |
| Random Forest | 98.59% |

### Final Model

Random Forest was selected as the final model because it achieved the highest predictive performance.

**Performance**

- Accuracy: 98.59%
- ROC-AUC Score: 0.997
- Cross Validation Accuracy: 96.77%

---

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Jupyter Notebook
- Joblib

---

## Project Structure

```
Loan_Approval_Prediction/
│
├── Loan_Approval.ipynb
├── loan_approved_dataset.csv
├── loan_approval_model.pkl
├── README.md
└── requirements.txt
```

---

## Sample Prediction

Input:

- Dependents: 2
- Education: Graduate
- Self Employed: No
- Annual Income: 9,000,000
- Loan Amount: 25,000,000
- Loan Term: 12
- CIBIL Score: 780
- Total Assets: 50,000,000

Prediction:

✅ Loan Approved

---

## Key Learnings

- Data preprocessing and feature engineering
- Label Encoding
- Model training and evaluation
- Hyperparameter tuning
- Cross-validation
- Model comparison and selection
- Saving trained models using Joblib

---

## Future Improvements

- Perform hyperparameter tuning to optimize the Random Forest model.
- Deploy the model using Streamlit.
- Test additional machine learning algorithms for comparison.

---

## Author

Garima Ghosh

Business Intelligence Developer | Data Analyst | Machine Learning Enthusiast