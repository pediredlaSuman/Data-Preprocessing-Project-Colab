# 🧹 Data Preprocessing Pipeline (DPP)


Original Project Colab file link : https://colab.research.google.com/drive/1awAvZSsBbyNKeqOUjT_IhnhV1eNF05e4?usp=sharing
This project demonstrates a complete data preprocessing pipeline for a student dataset using Python. It involves handling missing values, encoding categorical variables, discretization, outlier treatment, data visualization, normalization, and finally applying a basic machine learning model. The goal is to prepare real-world educational data for downstream analysis and classification.

> 📁 **File**: Student.csv  
> 🛠️ **Team**: Pediredla Suman (221020444), Co-author: 221000056  
> 🧪 **Tooling**: Python, Pandas, NumPy, Seaborn, Matplotlib, scikit-learn

---

## 🔍 Overview

This project focuses on end-to-end data preprocessing for a dataset of students' academic and demographic information. Tasks covered:

- Missing value imputation (mean, mode, median, EOD)
- Encoding (label & one-hot)
- Histogram/discretization (singleton, equal-width)
- Outlier detection and removal
- Correlation matrix and heatmap
- Basic classification using Decision Tree
- Skewness analysis & normalization insights

---

## 📊 Dataset Description

| Feature               | Description                                |
|-----------------------|--------------------------------------------|
| MathScore             | Student’s score in Math                    |
| ReadingScore          | Student’s score in Reading                 |
| WritingScore          | Student’s score in Writing                 |
| Gender                | Gender of the student                      |
| EthnicGroup           | Categorical variable for ethnicity         |
| ParentMaritalStatus   | Categorical variable on marital status     |
| NrSiblings            | Number of siblings                         |

---

## 🛠 Technologies Used

- **Python**
- **Pandas** – data handling
- **NumPy** – statistical operations
- **Matplotlib / Seaborn** – data visualization
- **Scikit-learn** – preprocessing + decision tree classification

---

## ⚙️ Pipeline Summary

### 🔧 Missing Value Handling
- **Mean Imputation** → `NrSiblings`
- **Mode Imputation** → `ReadingScore`, `EthnicGroup`
- **Median Imputation** → `MathScore`
- **EOD (End of Distribution)** → `WritingScore`

### 📊 Data Visualizations
- Histograms (before & after imputation)
- Bar graphs for binned values
- Scatter plots: Math vs Writing Scores
- Box plot for outlier detection
- Heatmap: Feature correlation

### 🔐 Encoding Techniques
- **Label Encoding** – categorical → numeric
- **One-Hot Encoding** – for `NrSiblings`

### 📉 Discretization
- Equal-width binning for continuous scores (e.g., MathScore)

### 🚫 Outlier Detection
- IQR-based outlier removal for `MathScore`

### 🔬 Skewness & Normalization
- Skewness check for `WritingScore`  
- Detection of distribution shape (right/left skew)

### 🤖 Classification Model
- **Model**: DecisionTreeClassifier
- **Features**: MathScore, WritingScore
- **Target**: Gender
- **Split**: 80% train / 20% test
- **Metrics**: Accuracy, Classification Report

---

## 📈 Key Outputs & Graphs

- ✅ **Histograms** (before/after imputation)
- ✅ **Bar Graphs** (binned scores)
- ✅ **Box Plot** (outlier detection)
- ✅ **Scatter Plot** (feature relationships)
- ✅ **Heatmap** (feature correlations)
- ✅ **Classification Report** (accuracy + precision/recall)
- ✅ **Skewness Statement** (data distribution insight)

---

## 📋 Results

- **Missing data handled** for all major columns
- **Encoding applied** correctly
- **Outliers identified and optionally removed**
- **Final accuracy** of Decision Tree Classifier:
- **Insights derived** from graphs, binning, and skewness analysis

---



