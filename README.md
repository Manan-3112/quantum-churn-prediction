# Quantum-Enhanced Customer Churn Prediction

A Quantum Machine Learning (QML) project that combines classical machine learning and quantum models to predict customer churn and generate customer risk assessments.

## Overview

This project develops a quantum-enhanced customer churn prediction system using customer banking data.

The system compares classical machine learning models with quantum machine learning approaches and combines their predictions to generate a final churn risk score.

## Project Workflow

1. Load and preprocess customer churn data.
2. Encode categorical features and engineer additional features.
3. Handle class imbalance using SMOTE.
4. Train classical machine learning models as benchmarks.
5. Select the most important features using Random Forest.
6. Reduce the selected features to 4 quantum features.
7. Scale quantum features for quantum circuit encoding.
8. Train Quantum Kernel SVM (QSVM).
9. Train a Variational Quantum Classifier (VQC).
10. Combine classical and quantum predictions using ensemble models.
11. Evaluate models using accuracy, AUC, F1-score and other classification metrics.
12. Generate customer-level churn risk scores and recommendations.
13. Provide an interactive customer churn prediction dashboard.

## Machine Learning Models

### Classical Models
- XGBoost
- Random Forest
- Logistic Regression
- XGBoost + Random Forest hybrid

### Quantum Models
- Quantum Kernel SVM (QSVM)
- Variational Quantum Classifier (VQC)
- Quantum-enhanced ensemble models

## Quantum Computing Approach

The quantum models use a 4-qubit architecture.

The project uses:

- ZZFeatureMap for quantum feature encoding
- RealAmplitudes variational ansatz
- Fidelity Quantum Kernel
- SPSA optimizer
- COBYLA optimizer
- Qiskit's StatevectorSampler

The four most important features identified through Random Forest are selected for the quantum models.

## Feature Engineering

Additional customer features are created, including:

- Balance-to-Salary Ratio
- Age Group
- Product Activity Score
- Credit Tier

Categorical features such as country and gender are also encoded before model training.

## Risk Assessment

The final system converts model predictions into a customer churn risk score from 0–100.

Risk levels:

- **Low Risk:** Score below 45
- **Medium Risk:** Score from 45 to 69
- **High Risk:** Score 70 and above

The system also provides recommended customer-retention actions based on the predicted risk level.

## Technologies

- Python
- Qiskit
- Qiskit Machine Learning
- Scikit-learn
- XGBoost
- Pandas
- NumPy
- Matplotlib
- Seaborn
- SHAP
- Imbalanced-learn
- SciPy
- Jupyter / Google Colab

## Repository Structure

```text
quantum-churn-prediction/
│
├── QML_Project_.ipynb
├── dataset.csv
├── README.md
└── requirements.txt
