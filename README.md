# MLE_CASE_STUDIES
Machine Learning Case Studies

This repository contains two machine-learning case studies using Logistic Regression to compare model performance with and without L2 regularization.

📁 Case Studies

Case Study 1 — Hospital Readmission Prediction

Dataset: diabetic_data.csv

The first case study uses hospital patient data to predict whether a patient will be readmitted.

Target Variable

The readmitted column is converted into a binary target:

NO → 0 (not readmitted)

>30 → 1 (readmitted)

<30 → 1 (readmitted)

Workflow

Import required Python libraries.

Load the diabetic patient dataset.

Replace ? values with missing values (NaN).

Check missing values, duplicate rows, data types, and target distribution.

Separate features (X) and target (y).

Split the data into training and testing sets using an 80/20 split.

Preprocess numerical and categorical features:

Numerical missing values are imputed.

Categorical missing values are imputed.

Categorical features are one-hot encoded.

Numerical features are standardized.

Train Logistic Regression:

Without L2 regularization.

With L2 regularization.

Evaluate both models using:

Accuracy

Classification report

ROC curve

AUC

Compare the final AUC values.

Case Study 2 — Credit Card Fraud Detection

Dataset: creditcard.csv

The second case study uses credit-card transaction data to classify transactions using the Class target variable.

Workflow

Import required Python libraries.

Load the credit-card dataset.

Inspect the dataset using head() and info().

Check for missing values.

Examine the target-class distribution and percentages.

Separate features (X) and target (y).

Split the data into training and testing sets using an 80/20 split with stratification.

Standardize the features using StandardScaler.

Train Logistic Regression:

Without L2 regularization.

With L2 regularization.

Generate probability predictions.

Calculate ROC curves and AUC scores.

Plot both ROC curves for comparison.

Calculate the difference between the two AUC scores.

🛠️ Technologies Used

Python 3

Pandas

NumPy

Matplotlib

Scikit-learn

Google Colab / Jupyter Notebook

📦 Installation

Install the required libraries with:

pip install pandas numpy matplotlib scikit-learn

▶️ How to Run

Open the corresponding notebook in Google Colab or Jupyter Notebook.

Upload the required dataset:

diabetic_data.csv for Case Study 1

creditcard.csv for Case Study 2

Run the notebook cells in order.

Review the printed evaluation metrics and ROC/AUC plots.

Note: The notebooks currently use /content/diabetic_data.csv and /content/creditcard.csv, which are paths commonly used in Google Colab.

📊 Model Comparison

Both case studies compare:

Model

Regularization

Main Evaluation

Logistic Regression

Without L2

ROC-AUC

Logistic Regression

With L2

ROC-AUC

The notebooks display the actual AUC values produced during execution rather than hard-coding results in this README.

📈 Evaluation

The primary comparison uses the ROC curve and Area Under the Curve (AUC).

ROC curve: Shows the relationship between the True Positive Rate and False Positive Rate across classification thresholds.

AUC: Summarizes the ROC curve into a single value for comparing the models' ability to distinguish between classes.

📂 Suggested Project Structure

project/
│
├── README.md
├── CASE_Study1
├── CASE_Study2
├── diabetic_data.csv
└── creditcard.csv

🎯 Learning Objectives

These case studies demonstrate:

Data loading and inspection

Data cleaning

Handling missing values

Feature preprocessing

Categorical feature encoding

Feature scaling

Train/test splitting

Binary classification

Logistic Regression

L2 regularization

ROC curves

AUC-based model comparison

👤 Author

Add your name, course, institution, and project details here.

Note: This README is based on the workflows implemented in the two provided case-study notebooks
