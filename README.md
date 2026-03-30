📱 Human Activity Recognition from Smartphone Sensors


📌 Project Overview

This project focuses on building a machine learning model to recognize human activities such as walking, sitting, standing, and lying using smartphone sensor data.

The project follows the complete data science lifecycle, including preprocessing, analysis, model building, evaluation, and deployment.

🎯 Objective
Classify human activities using sensor data
Build accurate predictive models
Deploy the model as an interactive application
📊 Dataset
Source: Kaggle
Dataset Name: Human Activity Recognition Dataset
🧾 Description:

The dataset contains sensor signals collected from smartphones placed on participants performing different activities.

📌 Features:
561 engineered features from:
Accelerometer
Gyroscope
Activity → Target variable
subject → Participant ID (removed during preprocessing)

📌 Activity Classes:
WALKING
WALKING_UPSTAIRS
WALKING_DOWNSTAIRS
SITTING
STANDING
LAYING

🧠 Project Workflow
🔹 Stage 1: Problem Definition & Literature Review
Studied Human Activity Recognition
Identified suitable ML models
🔹 Stage 2: Data Collection & Understanding
Loaded dataset from Kaggle
Explored structure and class distribution
🔹 Stage 3: Data Preprocessing & Cleaning
Removed subject column
Checked missing values (none found)
Encoded labels
Standardized features
🔹 Stage 4: Exploratory Data Analysis (EDA)
Activity distribution plots
Correlation heatmaps
Feature visualization
🔹 Stage 5: Feature Engineering & Selection
Selected top 50 important features
🔹 Stage 6: Model Building & Training

Models used:

Logistic Regression
Decision Tree
Random Forest
K-Nearest Neighbors
🔹 Stage 7: Model Evaluation & Comparison

Metrics:

Accuracy
Precision
Recall
F1-score

✅ Best Model: Random Forest

🔹 Model Interpretation & Explainability
Feature importance analysis
Confusion matrix
🔹 Deployment
Built using Streamlit
Real-time activity prediction interface
🔹 Stage 10: Documentation
GitHub repository
README
PPT presentation
🚀 Installation & Setup
pip install pandas numpy matplotlib seaborn scikit-learn streamlit joblib
▶️ Run the Project
1️⃣ Train Model
python train_model.py
2️⃣ Run App
streamlit run app.py
📁 Project Structure
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
📈 Results
Achieved accuracy: ~90–96%
Random Forest performed best
Balanced dataset improved model reliability
⚠️ Challenges
High dimensional data
Feature selection complexity
Similar activity patterns
🔮 Future Scope
Deep learning (LSTM, CNN)
Real-time mobile deployment
Larger dataset integration
