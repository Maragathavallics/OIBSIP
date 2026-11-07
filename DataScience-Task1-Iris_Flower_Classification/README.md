# 🌸 Iris Flower Classification

### Oasis Infobyte Internship – Task 1 | Data Science & Machine Learning

---

## 📌 Project Overview

This project focuses on developing a Machine Learning classification system to identify Iris flower species based on their physical measurements.

The model predicts one of three Iris species:

- Setosa
- Versicolor
- Virginica

The project follows a complete Machine Learning workflow, including data exploration, preprocessing, visualization, model training, hyperparameter optimization, cross-validation, and performance evaluation.

## 🎯 Objective

To build and evaluate classification models capable of accurately identifying Iris flower species using four numerical features:

- Sepal Length (cm)
- Sepal Width (cm)
- Petal Length (cm)
- Petal Width (cm)

## 📊 Dataset Information

**Dataset:** Iris Dataset

**Source:** `sklearn.datasets.load_iris()`

| Attribute | Details |
|---|---|
| Total Samples | 150 |
| Total Features | 4 |
| Target Classes | 3 |
| Samples per Class | 50 |
| Missing Values | None in the original dataset |

## 🛠️ Technologies & Libraries

| Technology | Purpose |
|---|---|
| Python | Programming language |
| NumPy | Numerical operations |
| Pandas | Data manipulation |
| Matplotlib | Data visualization |
| Seaborn | Statistical visualization |
| Scikit-learn | Machine Learning |
| Jupyter Notebook | Development environment |

## 🔍 Project Workflow

### 1. Data Loading
- Imported the Iris dataset using Scikit-learn.
- Converted the dataset into Pandas DataFrames.
- Examined dataset dimensions and feature information.

### 2. Exploratory Data Analysis (EDA)
- Analyzed dataset structure and data types.
- Checked missing values and duplicate records.
- Generated descriptive statistics.
- Visualized species distribution.
- Created pairplots and boxplots.
- Examined feature correlations using a heatmap.

### 3. Data Preprocessing
- Separated independent and dependent variables.
- Split the dataset into training and testing sets using an 80:20 ratio.
- Used stratified sampling to maintain class distribution.
- Applied feature scaling through StandardScaler within model pipelines where required.

### 4. Model Development

Seven Machine Learning classification algorithms were implemented and compared:

1. Logistic Regression
2. K-Nearest Neighbors (KNN)
3. Support Vector Machine (SVM)
4. Random Forest
5. Extra Trees Classifier
6. Gradient Boosting Classifier
7. Linear Discriminant Analysis (LDA)

### 5. Hyperparameter Optimization
- Applied GridSearchCV for hyperparameter tuning.
- Used stratified five-fold cross-validation.
- Selected the best parameter configuration for each model.
- Compared models using cross-validation accuracy and standard deviation.

### 6. Model Evaluation

The models were evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix

## 🏆 Best-Performing Model

**Selected Model: Support Vector Machine (SVM)**

The SVM model was selected based on its cross-validation performance and comparatively lower variation among the leading models.

### Performance Results

| Evaluation Metric | Result |
|---|---:|
| Mean CV Accuracy | 97.50% |
| CV Standard Deviation | 2.04% |
| Test Accuracy | 93.33% |
| Macro Precision | 0.93 |
| Macro Recall | 0.93 |
| Macro F1-score | 0.93 |

### Model Selection

Although Logistic Regression and Linear Discriminant Analysis achieved 100% test accuracy, SVM was selected based on its cross-validation performance and lower variation across folds.

The final test results for SVM showed:
- All 10 Setosa samples correctly classified.
- 9 out of 10 Versicolor samples correctly classified.
- 9 out of 10 Virginica samples correctly classified.

## 📈 Key Learnings

Through this project, I gained practical experience in:

- Data exploration and preprocessing.
- Exploratory Data Analysis.
- Statistical data visualization.
- Classification algorithms.
- Feature scaling and model pipelines.
- Hyperparameter tuning.
- Stratified cross-validation.
- Model comparison and evaluation.
- Interpreting confusion matrices and classification metrics.

<p align="center">
  ⭐ Learning • Building • Improving ⭐
</p>
