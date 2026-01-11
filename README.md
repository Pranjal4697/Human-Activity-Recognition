# Human Activity Recognition (HAR) using Machine Learning

A machine learning project that classifies human physical activities using wearable sensor data. The work emphasizes **feature engineering, model comparison, and real-world adaptability**, achieving **~90% accuracy** using classical ML algorithms.
 
**Tech Stack:** Python, Scikit-learn, TSFEL, NumPy, Pandas

---

## 🔍 Problem Overview

Human Activity Recognition (HAR) is a core problem in mobile computing, healthcare, and IoT systems. The challenge lies in handling **noisy multivariate time-series data** and extracting meaningful representations for reliable classification.

This project investigates:
- The impact of **feature engineering vs. raw sensor data**
- Performance trade-offs across **classical ML models**
- Generalization to **real-world sensor data**

---

## 📊 Dataset

- **UCI Human Activity Recognition Dataset**
- Smartphone accelerometer & gyroscope data
- 6 activities: Walking, Upstairs, Downstairs, Sitting, Standing, Laying
- 50 Hz sampling rate

---

## 🧠 Approach

### Data Processing
- Signal normalization and segmentation
- Noise handling for sensor stability

### Feature Engineering
- Extracted time-domain and frequency-domain features using **TSFEL**
- Reduced high-dimensional raw signals into compact representations

### Dimensionality Reduction
- Applied **PCA** to reduce redundancy
- Improved generalization and inference efficiency

### Models Implemented
- Decision Tree
- Random Forest
- Linear Regression (baseline comparison)

---

## 🚀 Results

| Model | Data Type | Accuracy |
|------|----------|----------|
| Decision Tree | Raw Sensor Data | ~78% |
| Decision Tree | TSFEL + PCA | ~88% |
| Random Forest | Raw Sensor Data | ~85% |
| **Random Forest** | **TSFEL + PCA** | **~90%** |

### Key Insights
- Feature engineering improves accuracy by **10–12%**
- Random Forest handles sensor noise and non-linear patterns effectively
- PCA reduces overfitting and improves scalability
- Raw time-series data performs poorly without domain-specific features

---

## 🌍 Real-World Validation

- Collected accelerometer data from a mobile device
- Applied the same preprocessing and feature pipeline
- Evaluated trained models on unseen real-world data
- Analyzed robustness and domain-shift effects

This step demonstrates **deployment awareness beyond offline benchmarks**.

---

