# employee-turnover-prediction-system

# Employee Turnover Prediction System

A Machine Learning-based system to predict **employee retention** (inverse of attrition) using workplace and HR data. The project uses classification algorithms—**Random Forest** and **Logistic Regression**—along with **feature selection** and **hyperparameter tuning** to improve model performance and interpretability.

---

## Project Overview

Organizations often struggle with employee attrition, which can result in high hiring and training costs. This system helps HR teams predict which employees are likely to leave (or stay), enabling proactive retention strategies.

---

## Dataset

- **Source:** [IBM HR Analytics Employee Attrition & Performance Dataset](https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset)
- **Filename:** `WA_Fn-UseC_-HR-Employee-Attrition.csv`
- Contains 35+ workplace-related features including:
  - Age, Job Role, Monthly Income
  - Distance from Home
  - Overtime status
  - Performance Rating, Job Satisfaction, Work-Life Balance, etc.

---

## ML Techniques Used

### Algorithms:
- **Random Forest Classifier**
- **Logistic Regression**

### Enhancements:
- **Feature Selection:** Used Recursive Feature Elimination (RFE) to select top features.
- **Hyperparameter Tuning:** Applied `GridSearchCV` for optimizing model parameters.
- **Standardization:** Scaled numeric features using `StandardScaler`.

---

## Model Evaluation

Both models were trained and evaluated using metrics such as:

- **Accuracy**
- **Precision**
- **Recall**
- **F1-score**
- **Confusion Matrix**

> Random Forest outperformed Logistic Regression in recall for identifying employees likely to leave (62% vs 55%).

---

## Results Snapshot

| Metric           | Logistic Regression | Random Forest     |
|------------------|---------------------|-------------------|
| Accuracy         | ~88%                | ~90%              |
| Recall (Leavers) | 55%                 | 62%               |
| Precision (Stay) | 90%                 | 92%               |

---

## Tech Stack

- Python
- pandas, numpy
- scikit-learn
- matplotlib / seaborn (optional for plots)

## How to Run

1. Clone the repository  
2. Install dependencies  
   ```bash
   pip install -r requirements.txt



