Machine Learning-Based Prediction of Ischemic Heart Disease Using Lipid Profile Parameters
Overview
This repository contains the complete analysis pipeline for predicting Ischemic Heart Disease (Cardiovascular Disease / CVD) using lipid profile and clinical parameters. Multiple machine learning models were trained, evaluated, and compared to identify the best-performing classifier for distinguishing Cases (IHD patients) from Controls (healthy individuals).
Dataset

Total samples: 929 (Cases: ~76.4%, Controls: ~23.6%)
Features: Gender, Age, BMI, Diabetes, Hypertension, Smoking, Triglycerides (TG), VLDL, LDL, HDL
Target variable: Case / Control (binary classification)
Train/Test split: 80% training, 20% testing (stratified)

Models Applied
ModelAccuracyAUC-ROCLightGBM0.96770.9987SVM (RBF Kernel)0.97850.9970XGBoost0.96240.9936Logistic Regression0.94620.9858Decision Tree0.94620.9334
Key Findings

LightGBM achieved the highest AUC-ROC (0.9987), making it the best overall model for CVD risk prediction.
The most important predictive features were: BMI, LDL, VLDL, Triglycerides, and Age — consistent with established cardiovascular risk factors.
All models demonstrated strong discriminative ability, confirming that lipid profiles are powerful biomarkers for IHD prediction.
