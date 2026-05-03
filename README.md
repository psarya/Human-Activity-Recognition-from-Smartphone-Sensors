# Human Activity Recognition System from Smartphone Sensor Data

## Project Overview

This project focuses on building a robust machine learning system to classify human activities using smartphone sensor data. The system leverages accelerometer and gyroscope signals to accurately recognize activities such as walking, sitting, standing, and lying. The project follows the complete data science lifecycle, including preprocessing, exploratory data analysis (EDA), feature engineering, model development, evaluation, and deployment.

## Objectives

Classify human activities using smartphone sensor data
Perform comprehensive exploratory data analysis
Build and compare multiple machine learning models
Identify the best-performing model
Deploy the model using an interactive Streamlit application
Dataset
Source: UCI HAR Dataset (via Kaggle)

The dataset contains 561 engineered features derived from:

Accelerometer signals
Gyroscope signals
Target Classes:

LAYING
SITTING
STANDING
WALKING
WALKING_DOWNSTAIRS
WALKING_UPSTAIRS
Methodology

### 1. Data Preprocessing

Removed irrelevant columns (e.g., subject identifiers)
Checked and handled missing values (none found in original datasets)
Encoded categorical activity labels using LabelEncoder
Standardized feature values using StandardScaler

### 2. Exploratory Data Analysis (EDA)

Visualized activity distribution
Generated correlation heatmaps for features
Identified feature relationships and patterns

### 3. Feature Engineering

Selected top 50 important features using SelectKBest with f_classif
Reduced dimensionality while preserving model performance

### 4. Model Building The following machine learning models were implemented:

Support Vector Machine (SVM)
Long Short-Term Memory (LSTM)
Random Forest

### 5. Model Evaluation Models were evaluated using:

Accuracy
Precision
Recall
F1-score
Confusion Matrix
Results & Comparison
Model	Accuracy
SVM	0.9006
Random Forest	0.8595
LSTM	0.9515

### Best Model:
LSTM ✔ Achieved highest accuracy (0.9515) and balanced performance across all classes

Model Interpretation
Activity distribution across the dataset was visualized.
Feature correlation heatmaps provided insights into relationships between sensor signals.
A confusion matrix for each model (SVM, Random Forest, LSTM) helps understand class-wise performance, showing where models might be confusing similar activities.
For Random Forest, feature importances indicate which sensor features contribute most to activity classification.

Deployment
The best-performing model is deployed using Streamlit.

🔗 Live Application: [https://wheat-amiable-impotent.ngrok-free.dev]

Features:
User input for sensor values (via CSV upload or manual sliders)
Real-time activity prediction
Interactive class probability visualization
Model performance analysis (accuracy comparison, feature importance, confusion matrix)
Simple and interactive UI
