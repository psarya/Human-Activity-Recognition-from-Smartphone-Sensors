# Human Activity Recognition System from Smartphone Sensor Data

## Project Overview
This project focuses on building a robust machine learning system to classify human activities using smartphone sensor data. The system leverages accelerometer and gyroscope signals to accurately recognize activities such as walking, sitting, standing, and lying.

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

| Model           | Accuracy |
|----------------|---------|
| SVM            | 0.9006  |
| Random Forest  | 0.8595  |
| LSTM           | 0.9515  |

### Best Model
**LSTM** achieved the highest accuracy (**95.15%**) and showed balanced performance across all activity classes.

---

## Model Interpretation
- Activity distribution was visualized to understand class balance  
- Correlation heatmaps revealed relationships between sensor features  
- Confusion matrices helped identify misclassifications between similar activities  
- Random Forest feature importance highlighted key contributing features  

---

## Deployment
The best-performing model is deployed using **Streamlit**.

### Live Application
https://wheat-amiable-impotent.ngrok-free.dev

### Features
- Upload sensor data via CSV or use manual input sliders  
- Real-time activity prediction  
- Interactive probability visualization  
- Model performance comparison  
- Feature importance and confusion matrix display  
- Clean and user-friendly interface  
