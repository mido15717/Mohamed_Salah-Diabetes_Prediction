# Diabetes Prediction Assignment

This project demonstrates the use of machine learning models to predict diabetes based on a dataset of medical features. The project explores multiple models, evaluates their performance, and applies techniques like standardization and regularization to improve accuracy.

## Table of Contents
1. Overview
2. Dataset
3. Models Used
4. Results
5. Experiment Report
6. Setup and Usage
7. Dependencies
8. License

## Overview
The goal of this project is to predict whether a patient has diabetes based on medical diagnostic measurements. The project uses Python and popular machine learning libraries to train and evaluate models.

## Dataset
The dataset used in this project is `diabetes.csv`, which contains the following features:
- Pregnancies
- Glucose
- BloodPressure
- SkinThickness
- Insulin
- BMI
- DiabetesPedigreeFunction
- Age
- Outcome (target variable: 0 = No Diabetes, 1 = Diabetes)

## Models Used
The following machine learning models were implemented and evaluated:
1. Logistic Regression
2. Decision Tree
3. Random Forest

Additionally, techniques like standardization and regularization (L1 and L2) were applied to improve model performance.

## Results
### Before Standardization
- **Logistic Regression**: Accuracy = 74.03%, Precision = 62%, Recall = 62%, F1-Score = 62%
- **Decision Tree**: Accuracy = 69.69%, Precision = 55%, Recall = 68%, F1-Score = 61%
- **Random Forest**: Accuracy = 74.02%, Precision = 62%, Recall = 66%, F1-Score = 64%

### After Standardization
- **Logistic Regression**: Accuracy = 73.59%, Precision = 62%, Recall = 62%, F1-Score = 62%
- **Decision Tree**: Accuracy = 69.69%, Precision = 55%, Recall = 69%, F1-Score = 61%
- **Random Forest**: Accuracy = 74.02%, Precision = 62%, Recall = 64%, F1-Score = 63%

### After Increasing Training Data
- **Decision Tree**: Accuracy = 75.97%, Precision = 65%, Recall = 71%, F1-Score = 68%
- **Logistic Regression**: Accuracy = 75.32%, Precision = 65%, Recall = 67%, F1-Score = 66%
- **Random Forest**: Accuracy = 75.32%, Precision = 65%, Recall = 67%, F1-Score = 66%

## Experiment Report
- **Best Performing Experiment**: The Decision Tree model performed the best after increasing the training data, achieving an accuracy of 75.97% and an F1-Score of 68%.

- **Challenges Faced**: 
  - Handling imbalanced data and ensuring fair evaluation of models.
  - Computational time for grid search and hyperparameter tuning.

- **Lessons Learned**:
  - Standardization improves the performance of Logistic Regression but has less impact on tree-based models.
  - Increasing the training data size significantly improves model performance.
  - Regularization (L1 and L2) helps in feature selection and prevents overfitting in Logistic Regression.

## Setup and Usage
1. Clone the repository:
   
2. Install the required dependencies:
    pip install -r requirements.txt

3. Run the Jupyter Notebook:
    jupyter notebook Diabetes.ipynb

4. Follow the steps in the notebook to train and evaluate the models.

Dependencies
The project requires the following Python libraries:

pandas
numpy
matplotlib
seaborn
scikit-learn

Install them using the requirements.txt file:

pandas
numpy
matplotlib
seaborn
scikit-learn
