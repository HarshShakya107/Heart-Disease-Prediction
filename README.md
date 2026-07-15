# Heart-Disease-Prediction
❤️ Heart Disease Prediction

An end-to-end machine learning project that predicts the likelihood of cardiovascular disease using patient health data. The pipeline covers data preprocessing, class-imbalance handling, hyperparameter optimization, model comparison, and experiment tracking.

📌 Overview

This project trains and compares three gradient boosting models — CatBoost, LightGBM, and XGBoost — to classify whether a patient has cardiovascular disease (cardio) based on clinical and lifestyle features (blood pressure, cholesterol, glucose, BMI, activity level, etc.).

🚀 Features


Data preprocessing — cleaning, encoding categorical features (bp_category) with LabelEncoder
Class imbalance handling — SMOTETomek (SMOTE + Tomek links) for balanced training data
Hyperparameter tuning — Optuna with TPESampler and MedianPruner, evaluated via 5-fold StratifiedKFold cross-validation
Model training — CatBoostClassifier, LGBMClassifier, XGBClassifier
Experiment tracking — all runs, params, metrics, and models logged with MLflow
Evaluation — Accuracy, Precision, Recall, F1 Score, ROC-AUC, Confusion Matrix, Classification Report
Feature importance analysis — per-model importance plots and CSV exports
Model comparison — side-by-side comparison table + bar chart, with inference time benchmarking
Model persistence — trained models, best params, and metrics saved via joblib


🛠️ Tech Stack

CategoryToolsLanguagePythonData handlingPandas, NumPyML ModelsCatBoost, LightGBM, XGBoostImbalance handlingimbalanced-learn (SMOTETomek)Hyperparameter tuningOptunaExperiment trackingMLflowVisualizationMatplotlibModel persistenceJoblib
