# Titanic Survival Prediction using Random Forest and Bagging Classifier

## Project Overview

This project implements ensemble learning techniques to predict passenger survival on the Titanic dataset.

The project explores and compares multiple ensemble-based classification approaches including Random Forest and Bagging Classifier with different base estimators.

The main goal is to understand how combining multiple machine learning models improves classification performance and reduces overfitting.

---

## Dataset Information

**Dataset:** Titanic Dataset

**Source:** Seaborn Dataset

### Target Variable

- Survived

### Features Used

- Passenger Class (Pclass)
- Gender (Sex)
- Age
- Fare
- Embarked

---

## Project Workflow

## 1. Data Loading

- Loaded Titanic dataset.
- Converted data into a structured format for analysis.

---

## 2. Data Preprocessing

Performed:

- Handling missing values
- Feature selection
- Encoding categorical variables
- Preparing data for model training

---

## 3. Train-Test Split

Dataset was divided into:

- Training Data
- Testing Data

for model evaluation.

---

# Machine Learning Models Implemented

## 1. Random Forest Classifier

Random Forest is an ensemble learning algorithm that combines multiple decision trees to improve prediction accuracy and reduce overfitting.

Implementation:

```python
RandomForestClassifier()
```

Parameters used:

```python
n_estimators = 201

max_depth = 4

oob_score = True
```

### Evaluation

Performance was measured using:

- Accuracy Score
- Out-of-Bag (OOB) Score

---

## 2. Bagging Classifier with Decision Tree

Bagging (Bootstrap Aggregating) trains multiple models on different subsets of data and combines their predictions.

Base Model:

```python
DecisionTreeClassifier()
```

Parameters:

```python
n_estimators = 201
```

Evaluation:

- Accuracy Score

---

## 3. Bagging Classifier with Logistic Regression

Bagging was also applied using Logistic Regression as the base estimator.

Base Model:

```python
LogisticRegression()
```

Parameters:

```python
n_estimators = 201
```

Evaluation:

- Accuracy Score

---

## Model Comparison

The project compares:

| Model | Base Algorithm |
|---|---|
| Random Forest | Decision Trees |
| Bagging Classifier | Decision Tree |
| Bagging Classifier | Logistic Regression |

This comparison helps understand the impact of ensemble methods on classification performance.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-Learn
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## Machine Learning Concepts Covered

- Ensemble Learning
- Random Forest
- Bagging
- Bootstrap Sampling
- Multiple Model Aggregation
- Classification
- Model Evaluation

---

## Results

The ensemble models successfully predicted Titanic passenger survival.

Random Forest and Bagging approaches demonstrated how combining multiple weak learners can improve model stability and generalization compared to individual models.

---

## Learning Outcomes

Through this project, I learned:

- Ensemble Learning Techniques
- Random Forest Algorithm
- Bagging Classifier
- Model Comparison
- Out-of-Bag Evaluation
- Classification Metrics
- Overfitting Reduction

---

## Installation

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

---

## Run Project

```bash
jupyter notebook
```

Open:

```text
RF_Bagging_classifier_on_titanic_dataset.ipynb
```

---

## Project Structure

```text
titanic-survival-prediction-random-forest-bagging
│
├── RF_Bagging_classifier_on_titanic_dataset.ipynb
├── README.md
└── requirements.txt
```

---

## Future Improvements

- Hyperparameter tuning using GridSearchCV
- Feature importance visualization
- Compare with XGBoost
- Deploy model using Streamlit
- Add ROC-AUC evaluation

---

## Author

Ashutosh Mehta

Computer Engineering Student

Machine Learning Enthusiast
