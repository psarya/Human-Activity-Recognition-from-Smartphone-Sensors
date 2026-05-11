## 🤖 LSTM Model — Results & Analysis

### Model Overview

The **Long Short-Term Memory (LSTM)** model is a recurrent neural network architecture well-suited for sequential sensor data. It captures temporal dependencies in accelerometer and gyroscope readings to classify human activities.

---

### 📊 Classification Report

| Class | Activity | Precision | Recall | F1-Score | Support |
|-------|----------|-----------|--------|----------|---------|
| 0 | Walking | 1.00 | 0.99 | 1.00 | 537 |
| 1 | Walking Upstairs | 0.97 | 0.80 | 0.88 | 491 |
| 2 | Walking Downstairs | 0.84 | 0.98 | 0.90 | 532 |
| 3 | Sitting | 0.87 | 1.00 | 0.93 | 496 |
| 4 | Standing | 1.00 | 0.91 | 0.95 | 420 |
| 5 | Laying | 0.94 | 0.87 | 0.91 | 471 |
| **Accuracy** | | — | — | **0.93** | 2947 |
| **Macro Avg** | | 0.94 | 0.93 | 0.93 | 2947 |
| **Weighted Avg** | | 0.94 | 0.93 | 0.93 | 2947 |

---

### 🔍 Key Observations

- **Overall Accuracy: 93%** across 2,947 test samples.
- **Class 0 (Walking)** achie
