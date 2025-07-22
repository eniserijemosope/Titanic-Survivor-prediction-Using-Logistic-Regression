# Titanic Survivor Prediction Using Logistic Regression

This project analyzes Titanic passenger data to predict survival outcomes using a **Logistic Regression** model. It involves **data cleaning**, **exploratory data analysis (EDA)**, **feature engineering**, and **model evaluation** to build a reliable binary classification model.

## Project Objectives

- Predict whether a passenger survived the Titanic disaster.
- Use logistic regression to classify survival (1 = Survived, 0 = Did not survive).
- Apply EDA and preprocessing to improve model accuracy and interpretability.

---

## Dataset

- **Source**: [Kaggle - Titanic: Machine Learning from Disaster](https://www.kaggle.com/c/titanic)
- **Features Used**:
  - `Pclass` (Ticket class)
  - `Sex`
  - `Age`
  - `SibSp` (Number of siblings/spouses aboard)
  - `Parch` (Number of parents/children aboard)
  - `Fare`
  - `Embarked`

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib & Seaborn (for EDA and visualization)
- Scikit-learn (for modeling)

## Data Cleaning & Preprocessing

- Handled missing values (`Age`, `Embarked`)
- Converted categorical features using one-hot encoding
- Scaled numerical features using `StandardScaler`
- Split data into training and testing sets (80/20)

## Exploratory Data Analysis (EDA)

EDA was conducted to understand:
- Class imbalance in the survival label
- Distribution of age, fare, class, and gender
- Correlation heatmaps for feature importance

## Model Used

- **Model**: Logistic Regression (`max_iter=1000`)
- **Reason**: Simple and effective for binary classification with interpretable coefficients.

## Performance Metrics

### Classification Report

| Class | Precision | Recall | F1-score | Support |
|-------|-----------|--------|----------|---------|
| **0** (Did not survive) | 0.81 | 0.90 | 0.85 | 163 |
| **1** (Survived)        | 0.81 | 0.66 | 0.73 | 104 |
| **Accuracy**            |       |       | **0.81** | 267 |
| **Macro avg**           | 0.81 | 0.78 | 0.79 | 267 |
| **Weighted avg**        | 0.81 | 0.81 | 0.80 | 267 |

## Key Takeaways

- Gender (`Sex`) and class (`Pclass`) were strong indicators of survival.
- Logistic Regression performs reasonably well with proper preprocessing.
- Feature scaling significantly improved convergence and accuracy.
