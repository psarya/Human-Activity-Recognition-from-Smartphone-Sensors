# Project Title: Human Activity Recognition System from Smartphone Sensor Data

## Team Members:
| Name            | Reg No |
| ----------------| ------ |
| Arya Suku       | —      |
| Arjun S         | 253105 |
| Ardra Selin A G | —      |
              

## Problem Statement
Human Activity Recognition (HAR) using smartphone sensor data is an essential predictive analytics task which provides benefits to healthcare and fitness tracking and smart environments. The sensors inside modern smartphones which include accelerometers and gyroscopes create continuous motion data through their measurement functions. This process of converting raw sensor data into accurate activity classifications presents on-going difficulties for researchers in the field.
The objective of this project is to develop a robust system that can accurately classify human physical activities—such as walking, sitting, standing, running, and stair climbing-using sensor data from smartphones. The project requires researchers to extract time-domain and frequency-domain features from the dataset and use Support Vector Machines (SVM), Random Forest and Long Short-Term Memory (LSTM) networks as machine learning models.

The project follows the complete data science lifecycle, including:
- Data preprocessing  
- Exploratory Data Analysis (EDA)  
- Feature engineering  
- Model development  
- Evaluation  
- Deployment using Streamlit  

---

## Objectives
- Classify human activities using smartphone sensor data  
- Perform comprehensive exploratory data analysis  
- Build and compare multiple machine learning models  
- Identify the best-performing model  
- Deploy the model using an interactive Streamlit application  

---

## Dataset
- **Source:** UCI HAR Dataset (via Kaggle)  
- The dataset contains **561 engineered features** derived from:

## Dataset Link:- 
- https://www.kaggle.com/datasets/uciml/human-activity-recognition-with-smartphones

### Feature Sources
- Accelerometer signals  
- Gyroscope signals  

### Target Classes
- LAYING  
- SITTING  
- STANDING  
- WALKING  
- WALKING_DOWNSTAIRS  
- WALKING_UPSTAIRS  

---

## Methodology

### 1. Data Preprocessing
- Removed irrelevant columns (e.g., subject identifiers)  
- Checked and handled missing values (none found)  
- Encoded activity labels using `LabelEncoder`  
- Standardized features using `StandardScaler`  

---

### 2. Exploratory Data Analysis (EDA)
- Visualized activity distribution  
- Generated correlation heatmaps  
- Identified feature relationships and patterns  

---

### 3. Feature Engineering
- Selected top 50 important features using `SelectKBest` with `f_classif`  
- Reduced dimensionality while maintaining performance  

---

### 4. Model Building
The following machine learning models were implemented:
- Support Vector Machine (SVM)  
- Random Forest  
- Long Short-Term Memory (LSTM)  

---

### 5. Model Evaluation
Models were evaluated using:
- Accuracy  
- Precision  
- Recall  
- F1-score  
- Confusion Matrix  

---

## Results & Comparison

| Model          | Accuracy|
|----------------|---------|
| SVM            | 0.9006  |
| Random Forest  | 0.8595  |
| LSTM           | 0.9515  |

### Best Model
**LSTM** achieved the highest accuracy (**95.15%**) and showed balanced performance across all activity classes.

---
## Evaluation Matrix
### Random Forest 
#### Classification Report
---

## Model Comparison
<img width="743" height="434" alt="Model Comparison" src="https://github.com/user-attachments/assets/5bf9d1cf-18ff-48fb-9cbc-3eedd1ac63ec" />

---

## Accuracy Comparison
<img width="687" height="465" alt="Model Accuracy Comaprison" src="https://github.com/user-attachments/assets/235a13ba-b191-4dcd-9d3f-638070c70934" />

---

## Model Performance Summary

### Support Vector Machine (SVM)
1.  **Accuracy:** Achieved a respectable accuracy of **90.06%**, demonstrating strong classification capabilities for the HAR dataset.
2.  **Precision/Recall/F1-Score:** The weighted average F1-score was **0.90**, indicating a good balance between precision and recall across classes.
3.  **Strengths:** Performed particularly well on 'LAYING' (100% precision and recall) and 'WALKING' activities, showing robustness in distinguishing these movements.

### Random Forest
1.  **Accuracy:** Had an accuracy of **85.95%**, slightly lower than SVM and LSTM but still a solid performance.
2.  **Precision/Recall/F1-Score:** The weighted average F1-score was **0.86**, reflecting its overall classification quality.
3.  **Strengths:** Showed high precision and recall for 'LAYING' and 'WALKING' activities. As an ensemble model, it's less prone to overfitting and provides feature importances, which can be valuable for interpretability.

### Long Short-Term Memory (LSTM)
1.  **Accuracy:** Achieved the highest accuracy among the three models at **95.15%**, highlighting its effectiveness for time-series sensor data.
2.  **Precision/Recall/F1-Score:** The weighted average F1-score was **0.95**, demonstrating superior overall performance in correctly classifying activities.
3.  **Strengths:** Excels in capturing temporal dependencies within the sensor data, leading to better distinction between similar activities and achieving top performance across almost all metrics. It showed excellent performance across all individual activities as well.

---

## Conclusion
This project successfully developed and deployed a Human Activity Recognition system capable of classifying six common activities from smartphone sensor data. By leveraging a combination of traditional machine learning models (SVM, Random Forest) and deep learning (LSTM), we achieved high accuracy, with the LSTM model demonstrating superior performance. The deployment of an interactive Streamlit application further enhances the utility and accessibility of the model, providing real-time predictions and interpretability. This project serves as a comprehensive example of a complete machine learning pipeline, from data analysis and model development to deployment and evaluation.

---

## Application Screenshots
### Home Interface
<img width="1892" height="599" alt="Screenshot 2026-05-03 225913" src="https://github.com/user-attachments/assets/82d547a6-b25b-45cb-babd-8a9ad16a7610" />

### File Upload & Predictions
<img width="1879" height="965" alt="File upload   Prediction" src="https://github.com/user-attachments/assets/0ef2569e-b98a-4a9f-b20a-40e497ef14cb" />

### Manual Feature Input
<img width="1890" height="971" alt="Screenshot 2026-05-03 225135" src="https://github.com/user-attachments/assets/91969b16-1936-4c4d-b879-993900efad6e" />

### Model Performance & explainability
<img width="1882" height="929" alt="Screenshot 2026-05-03 225817" src="https://github.com/user-attachments/assets/93279b3a-79d8-4935-8767-6108248dea1d" />

### About
<img width="1889" height="884" alt="Screenshot 2026-05-03 225842" src="https://github.com/user-attachments/assets/ef0f5cf4-9261-4b64-b2ac-e6356bd7659c" />

---

## Deployment
- The best-performing model is deployed using **Streamlit**.

### Live Application
- https://wheat-amiable-impotent.ngrok-free.dev

### Features
- Upload sensor data via CSV or use manual input sliders  
- Real-time activity prediction  
- Interactive probability visualization  
- Model performance comparison  
- Feature importance and confusion matrix display  
- Clean and user-friendly interface  
