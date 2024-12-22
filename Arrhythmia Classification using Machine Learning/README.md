# Arrhythmia Prediction and Classification

This project focuses on predicting and classifying arrhythmias using various machine learning algorithms. The dataset is sourced from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Arrhythmia) and consists of 452 examples distributed across 16 different classes.

## Dataset Overview

- **Number of Examples:** 452  
- **Number of Features:** 279 (e.g., age, sex, weight, height, and various medical parameters)  
- **Classes:** 16 total (12 arrhythmia types + 1 normal group)  
  - 245 examples labeled as "normal"
  - Remaining examples represent arrhythmia types, such as "coronary artery disease" and "right bundle branch block"

## Objective

The goal of this project is to:
1. Predict whether a person is suffering from arrhythmia.
2. Classify the type of arrhythmia into one of the 12 available groups.

## Algorithms Used

The following machine learning algorithms were implemented for classification:

- **K-Nearest Neighbors (KNN) Classifier**  
- **Logistic Regression**  
- **Decision Tree Classifier**  
- **Linear Support Vector Classifier (SVC)**  
- **Kernelized Support Vector Classifier (SVC)**  
- **Random Forest Classifier**  
- **Principal Component Analysis (PCA)** (for dimensionality reduction)

## Project Workflow

### Step 1: Data Exploration
- Analyzed the 279 features to identify patterns and correlations.
- Addressed the challenge of high dimensionality with a limited dataset using PCA.

### Step 2: Data Preprocessing
- Handled missing values, standardized data, and prepared it for modeling.
- Applied PCA to:
  - Reduce feature space dimensionality.
  - Eliminate collinearity.
  - Improve execution time and model performance.

### Step 3: Model Training and Evaluation
- Trained various machine learning algorithms.
- Evaluated model performance using accuracy, recall, and other metrics.

### Step 4: Model Tuning with PCA
- PCA reduced dataset complexity, enhancing model accuracy and mitigating overfitting.
- Retrained models on PCA-transformed data, achieving significant performance improvements.

## Results
![result](https://github.com/user-attachments/assets/86bd2055-2222-4bfc-b3ba-878418dc51bb)



- **Best-Performing Model:** Kernelized Support Vector Machine (SVM) with PCA  
- **Accuracy:** 80.21%  
- **Highlights of PCA:**  
  - Reduced dimensionality and collinearity.  
  - Prioritized high-variance variables for improved predictions.  
  - Enhanced model execution time and accuracy.

## Conclusion

Principal Component Analysis (PCA) proved to be a powerful technique for handling high-dimensional data, addressing collinearity, and optimizing model performance. The Kernelized SVM with PCA achieved the best results, highlighting the effectiveness of dimensionality reduction in improving recall and accuracy for arrhythmia prediction and classification.

---
