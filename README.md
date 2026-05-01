# Semiconductor-yield-prediction-ml
Machine learning project to predict semiconductor manufacturing pass/fail yield using sensor data, with preprocessing, model comparison, and hyperparameter tuning.

# Semiconductor Manufacturing Yield Prediction Using Machine Learning

## 📌 Project Overview
This project focuses on predicting whether a semiconductor product will **Pass (-1)** or **Fail (1)** quality testing using sensor data collected during the manufacturing process. Machine Learning techniques are applied to analyze the data, build models, and identify the best-performing classifier.

---

## 🎯 Objective
- Build a classification model to predict Pass/Fail yield
- Handle high-dimensional sensor data
- Compare multiple machine learning models
- Optimize model performance using hyperparameter tuning
- Select and save the best model

---

## 📂 Dataset
- File: `signal-data.csv`
- Rows: 1567
- Columns: 592  
  - 591 sensor features  
  - 1 target column (Pass/Fail)

### Target Variable:
- `-1` → Pass  
- `1` → Fail  

---

## ⚙️ Technologies Used
- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- Imbalanced-learn (SMOTE)
- Joblib

---

## 🔄 Project Workflow

### 1. Data Understanding
- Loaded dataset
- Checked shape, columns, and data types
- Analyzed target distribution

### 2. Data Cleaning
- Removed timestamp column
- Handled missing values using mean imputation

### 3. Data Analysis
- Performed statistical analysis
- Visualized feature distributions and relationships

### 4. Data Preprocessing
- Separated features (X) and target (y)
- Balanced dataset using SMOTE
- Split data into training and testing sets
- Applied feature scaling using StandardScaler

### 5. Model Training
Trained and evaluated:
- Random Forest
- Support Vector Machine (SVM)
- Naive Bayes

### 6. Model Tuning
- Applied GridSearchCV on Random Forest
- Found optimal hyperparameters

### 7. Model Evaluation
- Compared model accuracies
- Tuned Random Forest achieved highest accuracy (~99%)

### 8. Model Saving
- Final model saved using Joblib:
---

## 📊 Results
- Tuned Random Forest Accuracy: **~99%**
- High precision, recall, and F1-score for both classes
- Balanced and reliable performance

---

## 🏆 Final Model
- **Tuned Random Forest Classifier**
- Selected based on highest accuracy and performance

---

## 💾 How to Run

1. Upload dataset (`signal-data.csv`)
2. Run the notebook step by step
3. Train models and evaluate results
4. Final model will be saved automatically

---

## 📌 Output
- Model comparison table
- Classification reports
- Saved trained model (`.pkl` file)

---

## 🚀 Conclusion
The project successfully demonstrates how machine learning can be used to predict semiconductor manufacturing yield using sensor data. The optimized Random Forest model provides highly accurate and reliable predictions.

---
