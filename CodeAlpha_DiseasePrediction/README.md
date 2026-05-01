# CodeAlpha_DiseasePrediction

# Disease Prediction from Medical Data
### CodeAlpha Machine Learning Internship - Task 4

## Overview
Built a machine learning model to predict whether a patient has heart disease
based on medical measurements like age, cholesterol, blood pressure and more.

Dataset used: [Heart Disease Dataset](https://www.kaggle.com/datasets/johnsmith88/heart-disease-dataset) from Kaggle  
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
| Logistic Regression | 0.82      | 0.81   | 0.81     | 0.930   |
| Decision Tree       | 0.87      | 0.87   | 0.87     | 0.933   |
| Random Forest       | 1.00      | 1.00   | 1.00     | 1.000   |

Decision Tree had the best honest ROC-AUC score (0.933).
Random Forest scored perfect 1.0 which indicates overfitting on the test set.

---

## Project Structure
```
CodeAlpha_DiseasePrediction/
├── data/                  # dataset goes here (not uploaded - see link above)
├── reports/
│   └── figures/           # saved plots
├── disease_prediction.ipynb
└── README.md
```

---

## How to Run

1. Download the dataset from the Kaggle link above
2. Place `heart.csv` inside the `data/` folder
3. Open `disease_prediction.ipynb` in Jupyter Notebook
4. Run all cells from top to bottom

---

## Libraries Required

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

---

## Key Takeaways

- Balanced dataset made evaluation straightforward — accuracy is reliable here
- Random Forest overfitting is a red flag, not a good result
- Decision Tree correctly identified 94 out of 105 actual disease cases
- In medical prediction, recall matters more than accuracy —
  missing a sick patient is worse than a false alarm
