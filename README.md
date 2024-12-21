# Health Admission Prediction Project

## **Project Overview**

This project is part of my **final assignment** for the **"Introduction to AI & Data Science"** course at the **Faculty of Computer Science, Universitas Indonesia**. The goal is to analyze and predict hospital admission outcomes using machine learning techniques. The dataset includes various features related to patient demographics, medical conditions, lab results, and outcomes during their hospital stay.

The project applies **Exploratory Data Analysis (EDA)** for data visualization and analysis, followed by **machine learning** models to predict patient outcomes, such as discharge, expiry, or DAMA (Discharged Against Medical Advice).

## **Project Objectives**

The key objectives of this project are to:

- **Analyze health admission data** to uncover patterns and relationships between patient demographics, medical conditions, and hospital outcomes.
- **Apply machine learning techniques** to predict patient outcomes (e.g., discharge, expiry) based on factors such as age, gender, smoking habits, medical history, and lab results.
- **Use statistical analysis and data visualization** to explore the data and provide meaningful insights.
- **Apply clustering techniques** to analyze and identify different groups of patients based on their characteristics and outcomes.

## **Methodology**

### 1. **Data Preprocessing**

### 2. **Exploratory Data Analysis (EDA)**

### 3. **Classification Models**

The classification task is aimed at predicting categorical outcomes such as whether a patient will be **discharged** or face **expiry**. Several classification models were tested for this task, including:

- **Random Forest Classifier**
- **Naive Bayes Classifier (Bernoulli)**
- **K-Nearest Neighbor (KNN)**

These models are suitable for mixed input types (nominal and categorical) and can handle **multi-class outputs** (more than two categories).

### **Handling Imbalanced Classes**

Since the dataset may have imbalanced classes (i.e., some outcomes may occur more frequently than others), several **oversampling** and **undersampling** techniques were applied to balance the class distribution:

- **Random Oversampling**
- **Borderline-SMOTE**
- **SMOTE**
- **ADASYN**
- **Random Undersampling**
- **Tomek Links**

### **Best Performing Model for Classification:**

After evaluating various classification models, the **Random Forest Classifier** with **Tomek Links** and **Random Undersampling** was found to provide the best performance. Below are the results and rationale behind the choice of the model:

- **Random Forest with Tomek Links:**
    - **Accuracy**: 0.93
    - **Recall**: 0.63
- **Random Forest with Random Undersampler:**
    - **Accuracy**: 0.77
    - **Recall**: 0.79

### **Why High Recall?**

We chose to prioritize **Recall** over **Accuracy** in this project, as the primary concern in health admission prediction is minimizing **false negatives**. A high **Recall** value ensures that fewer critical cases are missed, especially for outcomes like **Expiry**. A false negative in this case, where a seriously ill patient is misclassified as healthy, could have severe consequences and compromise patient safety. Therefore, **Recall** is a key metric in healthcare predictions, where identifying every possible risk is crucial for the wellbeing of patients.

### 4. **Regression Models**

For continuous outcome prediction (e.g., **duration of hospital stay**), the following regression models were tested:

- **Linear Regression**
- **Lasso Regression**
- **Ridge Regression**
- **SVR (Support Vector Regression)**
- **Decision Tree Regression**
- **Random Forest Regression**

### **Best Performing Model for Regression**

The **Random Forest Regression** model performed the best, achieving:

- **Mean Squared Error (MSE)**: 0.0015 (lowest)
- **Root Mean Squared Error (RMSE)**: 0.039 (lowest)
- **R-Squared (R²)**: 0.648 (highest)
- **Mean Absolute Error (MAE)**: 0.024 (lowest)

### 5. **Clustering Models**

To analyze patterns and group patients into different clusters, the following clustering techniques were applied:

- **K-Means Clustering.**
- **K-Means Clustering without PCA**
- **Agglomerative Clustering**
- **DBSCAN (Density-Based Spatial Clustering of Applications with Noise)**
