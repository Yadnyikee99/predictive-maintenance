Predictive Maintenance Using Bearing Fault Diagnosis
Overview

This project focuses on predictive maintenance using machine learning techniques for bearing fault diagnosis across multiple datasets. The study combines feature engineering, exploratory data analysis (EDA), and classification models to identify bearing health conditions and evaluate cross-domain generalization.

The project utilizes vibration signal datasets from:

IMS Bearing Dataset, 
IMS Cross-Domain Dataset, 
XJTU-SY Bearing Dataset

The main objective is to develop a scalable and reliable fault diagnosis pipeline capable of identifying bearing conditions using statistical vibration features.

Problem Statement

Industrial rotating machinery heavily depends on rolling element bearings for smooth operation. Unexpected bearing failures can lead to:

Production downtime
Increased maintenance costs
Equipment damage
Safety risks

Traditional maintenance strategies such as reactive and preventive maintenance are often inefficient because they either respond after failure occurs or rely on fixed maintenance schedules.

This project aims to build an intelligent predictive maintenance framework using machine learning models that can detect bearing faults early using vibration signal analysis.

Objectives
Perform vibration signal preprocessing and feature extraction
Conduct exploratory data analysis on bearing datasets
Compare time-domain and frequency-domain features
Train machine learning models for bearing fault classification
Evaluate cross-domain generalization performance
Identify the most important statistical vibration features
Research Questions
RQ1

How effectively can statistical vibration features classify bearing faults across multiple datasets?

RQ2

Which statistical vibration features contribute most to accurate bearing fault prediction?

RQ3

How does model performance vary between time-domain and frequency-domain features?

RQ4

Can machine learning models trained on one dataset generalize to another dataset in cross-domain fault diagnosis?

Datasets Used
IMS Bearing Dataset

The IMS dataset contains run-to-failure bearing vibration signals collected from rotating machinery under controlled conditions.

IMS Cross-Domain Dataset

Used for evaluating domain adaptation and model generalization.

XJTU-SY Bearing Dataset

A widely used benchmark dataset for intelligent fault diagnosis research.

Feature Engineering

The following statistical features were extracted from vibration signals:

Time-Domain Features
Mean
Standard Deviation
RMS
Variance
Skewness
Kurtosis
Peak-to-Peak
Crest Factor
Shape Factor
Impulse Factor
Frequency-Domain Features
Spectral Mean
Spectral Entropy
Dominant Frequency
Frequency Variance
FFT-based Statistical Features
Exploratory Data Analysis (EDA)

EDA was performed to:

Analyze feature distributions
Detect missing values
Identify outliers
Study class imbalance
Understand correlations between features
Compare healthy and faulty bearing conditions

Visualization techniques included:

Histograms
Boxplots
Heatmaps
Correlation matrices
Feature importance plots

Project Structure

predictive-maintenance-project/
│
├── data/
│   ├── ims_features.csv
│   ├── ims_crossdomain.csv
│   ├── xjtu_features.csv
│
├── notebooks/
│   ├── preprocessing.ipynb
│   ├── eda.ipynb
│   ├── model_training.ipynb
│
├── results/
│   ├── confusion_matrix.png
│   ├── feature_importance.png
│   ├── correlation_heatmap.png
│
├── README.md
├── requirements.txt


Key Findings
Statistical vibration features are highly effective for bearing fault diagnosis.
Time-domain features outperform frequency-domain features.
Random Forest achieved near-perfect classification accuracy.
Cross-domain datasets help evaluate real-world model robustness.
Feature engineering significantly improves predictive performance.
Future Scope

Potential future improvements include:

Deep learning-based fault diagnosis
Transfer learning for domain adaptation
Real-time predictive maintenance systems
Edge AI deployment for industrial monitoring
Explainable AI for fault interpretation
Applications

This project can be applied in:

Manufacturing industries
Smart factories
Industrial IoT systems
Rotating machinery monitoring
Aerospace maintenance
Automotive predictive maintenance
Energy and power plants
Author

Yadnikee

Data Science and Machine Learning Research Project

License

This project is intended for academic and research purposes.


