# Human Activity Recognition System from Smartphone Sensor Data

## Project Overview
This project focuses on building a robust machine learning system to classify human activities using smartphone sensor data. The system leverages accelerometer and gyroscope signals to accurately recognize activities such as walking, sitting, standing, and lying.
The project follows the complete data science lifecycle, including preprocessing, exploratory data analysis (EDA), feature engineering, model development, evaluation, and deployment.

---

 ## Objectives
- Classify human activities using smartphone sensor data  
- Perform comprehensive exploratory data analysis  
- Build and compare multiple machine learning models  
- Identify the best-performing model  
- Deploy the model using an interactive Streamlit application  

---

 ## Dataset
**Source:** UCI HAR Dataset (via Kaggle)

The dataset contains **561 engineered features** derived from:
- Accelerometer signals  
- Gyroscope signals  

 Target Classes:
- WALKING  
- WALKING_UPSTAIRS  
- WALKING_DOWNSTAIRS  
- SITTING  
- STANDING  
- LAYING  

---
## Methodology

**1. Data Preprocessing**
- Removed irrelevant columns (e.g., subject identifiers)  
- Checked and handled missing values  
- Encoded categorical activity labels  
- Standardized feature values  

---

**2. Exploratory Data Analysis (EDA)**
- Visualized activity distribution  
- Generated correlation heatmaps  
- Identified feature relationships and patterns  

---

 **3. Feature Engineering**
- Selected top 50 important features using feature selection techniques  
- Reduced dimensionality while preserving model performance  

---

**4. Model Building**
 The following machine learning models were implemented:

- SVM 
- LSTM 
- Random Forest    

---

 **5. Model Evaluation**
 Models were evaluated using:

- Accuracy  
- Precision  
- Recall  
- F1-score  

---

## Results & Comparison

| Model               | Accuracy |
|---------------------|----------|
| SVM                 | 0.90     |
| LSTM                | 0.85     |
| Random Forest       | 0.96     |


**Best Model:** 
✔ Achieved highest accuracy and balanced performance across all classes  

---

## Model Interpretation
- 
-  
-  

---

## Deployment
The best-performing model is deployed using Streamlit.

### 🔗 Live Application:


### Features:
- User input for sensor values  
- Real-time activity prediction  
- Simple and interactive UI  

---


