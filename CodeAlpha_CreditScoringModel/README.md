# CodeAlpha_CreditScoringModel

# Credit Scoring Model
### CodeAlpha Machine Learning Internship - Task 1

## Overview
Built a machine learning model to predict whether a loan applicant is likely to default based on their financial history.

Dataset used: [Give Me Some Credit](https://www.kaggle.com/datasets/brycecf/give-me-some-credit-dataset) from Kaggle  
Language: Python  
Notebook: Jupyter Notebook

---

## Models Used
- Logistic Regression
- Decision Tree
- Random Forest

---

## Results

| Model               | Precision | Recall | F1-Score | ROC-AUC |
|---------------------|-----------|--------|----------|---------|
| Logistic Regression | 0.62      | 0.05   | 0.10     | 0.813   |
| Decision Tree       | 0.60      | 0.15   | 0.24     | 0.848   |
| Random Forest       | 0.57      | 0.20   | 0.30     | 0.840   |

Decision Tree had the best ROC-AUC score (0.848).

---

## Project Structure
CodeAlpha_CreditScoringModel/
├── data/                  # dataset goes here (not uploaded - see link above)
├── reports/
│   └── figures/           # saved plots
├── credit_scoring.ipynb   # main notebook
└── README.md

---

## How to Run

1. Download the dataset from the Kaggle link above
2. Place `cs-training.csv` inside the `data/` folder
3. Open `credit_scoring.ipynb` in Jupyter Notebook
4. Run all cells from top to bottom

---

## Libraries Required
pip install pandas numpy matplotlib seaborn scikit-learn

---

## Key Takeaways

- Accuracy is misleading on imbalanced datasets — ROC-AUC is more reliable
- Missing value treatment and outlier capping improved model stability
- Decision Tree outperformed Random Forest on this dataset by ROC-AUC