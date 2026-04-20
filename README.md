Human Activity Recognition from Smartphone Sensors
Project Summary

This project develops a machine learning system to recognize human activities such as walking, sitting, standing, and lying using smartphone sensor data. The work follows a complete data science pipeline, including preprocessing, analysis, model building, evaluation, and deployment.

Objective
Classify human activities using sensor data
Build and compare multiple machine learning models
Deploy the best performing model as an interactive application
Dataset
Source: Kaggle – Human Activity Recognition Dataset
The dataset contains 561 engineered features derived from:
Accelerometer
Gyroscope
Target Classes
WALKING
WALKING_UPSTAIRS
WALKING_DOWNSTAIRS
SITTING
STANDING
LAYING
Project Workflow
Data Preprocessing
Removed unnecessary columns such as subject
Verified absence of missing values
Encoded activity labels
Standardized feature values
Exploratory Data Analysis
Analyzed class distribution
Generated correlation heatmaps
Visualized feature patterns
Feature Engineering
Selected the top 50 important features to reduce dimensionality
Model Building

The following models were implemented and compared:

Logistic Regression
Decision Tree
Random Forest
K-Nearest Neighbors
Results and Evaluation

Models were evaluated using:

Accuracy
Precision
Recall
F1-score

The Random Forest model performed best with an accuracy of approximately 90–96 percent and provided balanced performance across all classes.

Deployment

The final model is deployed using Streamlit, providing an interactive interface for real-time activity prediction.

Project Structure
HAR_Project/
│
├── app.py
├── train_model.py
├── train.csv
├── test.csv
├── har_model.pkl
├── scaler.pkl
├── selector.pkl
├── label_encoder.pkl
├── feature_columns.pkl
├── README.md
└── requirements.txt
Installation and Setup

Install the required dependencies:

pip install pandas numpy matplotlib seaborn scikit-learn streamlit joblib
Running the Project

Train the model:

python train_model.py

Run the application:

streamlit run app.py
Challenges
High dimensionality of data
Complexity in feature selection
Similar patterns between different activities
Future Work
Implementation of deep learning models such as LSTM and CNN
Real-time mobile deployment
Integration of larger datasets
Conclusion

This project demonstrates the effectiveness of machine learning techniques in recognizing human activities using smartphone sensor data. The system achieves high accuracy and provides a practical solution through an interactive application.

 Team Members
- Ardra Selin A G (ardraselin22)
- Arjun S (arjuns-oss)
- Arya Suku (psarya)

## Model Results & Comparison

| Model                | Accuracy |
|---------------------|----------|
| Logistic Regression | ~90%     |
| Decision Tree       | ~87%     |
| Random Forest       | ~96%     |
| KNN                 | ~91%     |

## 🌐 Live Deployment
https://wheat-amiable-impotent.ngrok-free.dev

Course: Predictive Analytics 2025-26
