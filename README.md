# 📚 Student Performance Factors: A Machine Learning Analysis

## 📌 Project Overview
This project explores various factors that influence a student's academic success and builds machine learning models to predict whether a student will pass or fail their exams based on these features. The goal is to uncover key academic, personal, and socioeconomic drivers of student performance to better understand how to support learners.

## 🗄️ Dataset
* **Source:** Simulated student performance dataset by *lainguyn123* on Kaggle.
* **Size:** 6,607 student records.
* **Features Analyzed (20 total):** Includes academic habits (`Hours_Studied`, `Attendance`, `Previous_Scores`), personal characteristics (`Motivation_Level`, `Gender`), and socioeconomic factors (`Parental_Involvement`, `Access_to_Resources`, `Family_Income`). 

## 🛠️ Methodology & Tools
1. **Data Preprocessing:** 
   * Imputed missing numerical values with column means and missing categorical values with the mode.
   * Converted the target variable (`Exam_Score`) into a binary `Pass_Fail` classification based on the median score.
   * Encoded categorical variables and standardized numeric features using `StandardScaler`.
2. **Class Balancing:** Addressed class imbalances in the target variable using the Synthetic Minority Over-sampling Technique (SMOTE).
3. **Model Evaluation:** Evaluated five classifiers (Logistic Regression, Decision Tree, Random Forest, SVM, and K-Nearest Neighbors) using an 80/20 train-test split.

## 📊 Key Findings & Model Performance
* **K-Nearest Neighbors (KNN):** Achieved an optimal accuracy of 87% when utilizing $k=11$ neighbors. 
* **Logistic Regression:** Delivered strong predictive performance with an accuracy of 89% and an impressive ROC AUC score of 0.966.
* **Decision Tree:** Achieved an optimal accuracy of 84% at a tree depth of 7.

## 📁 Repository Structure
* `student-performance-factors.ipynb`: The complete Python codebase containing exploratory data analysis, data cleaning, SMOTE application, and model evaluation metrics.
* `StudentPerformanceFactors.csv`: The dataset used for model training and testing.
