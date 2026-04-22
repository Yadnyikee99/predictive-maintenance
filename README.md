Predictive Maintenance using Machine Learning
Overview

This project focuses on early fault detection in rotating machinery using the IMS bearing dataset.
The goal is to identify failures as early as possible by analyzing time-domain and frequency-domain signals.

It explores whether advanced feature engineering and machine learning models can improve Time-to-Detection (TTD) and overall reliability.

Objectives
Compare time-domain vs frequency-domain features
Evaluate early fault detection capability
Analyze whether feature fusion improves performance
Build a robust ML pipeline for predictive maintenance

Dataset
Source: IMS Bearing Dataset

Data Type: Vibration signals over time

Features Extracted:
Time-domain: RMS, Mean, Std, Kurtosis
Frequency-domain: FFT Energy, Spectral Entropy

Target:
Remaining Useful Life (RUL)
Fault detection labels

Methodology
1. Data Preprocessing
Timestamp extraction & sorting
Noise handling
Label generation (RUL / failure threshold)
2. Feature Engineering
Statistical features (mean, variance, etc.)
Signal-based features (FFT, entropy)
Feature selection to remove redundancy
3. Model Building
Machine Learning models used:
Random Forest
XGBoost
Logistic Regression (baseline)
4. Evaluation Metrics
Time-to-Detection (TTD)
Accuracy / F1 Score
Detection delay

Key Results
Frequency-domain features showed earlier fault detection
Combined features improved model stability
Tree-based models performed best for this dataset
