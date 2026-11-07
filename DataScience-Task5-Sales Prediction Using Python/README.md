# 📈 Sales Prediction Using Python

<p align="center">
  **Oasis Infobyte – Data Science Internship | Task 5**
</p>

## 📌 Project Overview

Sales Prediction Using Python is a Machine Learning project that analyzes the relationship between advertising expenditure and product sales.

The project uses advertising data from three different marketing channels: TV, Radio, and Newspaper. By applying regression techniques, the objective is to understand how advertising expenditure relates to sales and predict sales using Machine Learning models.

Two regression algorithms, Linear Regression and Polynomial Regression, are implemented and evaluated to identify the better-performing model.

## 🎯 Project Objectives

- Understand and analyze the advertising dataset.
- Perform data cleaning and preprocessing.
- Conduct Exploratory Data Analysis (EDA).
- Analyze the relationship between advertising expenditure and sales.
- Visualize correlations between different variables.
- Implement Linear Regression for sales prediction.
- Implement Polynomial Regression as an additional model.
- Evaluate both models using regression performance metrics.
- Compare model performance and identify the better-performing algorithm.

## 🛠️ Technologies & Libraries Used

| Technology | Purpose |
|---|---|
| Python | Programming language |
| Pandas | Data manipulation and analysis |
| NumPy | Numerical computations |
| Matplotlib | Data visualization |
| Seaborn | Statistical visualization |
| Scikit-learn | Machine Learning and model evaluation |
| Google Colab | Development environment |

## 📂 Dataset Information

**Dataset Name:** Advertising.csv

The dataset contains advertising expenditure across three marketing channels and the corresponding product sales.

**Dataset Overview:**
- Total Records: 200
- Total Columns: 4
- Target Variable: Sales
- Input Features: TV, Radio, Newspaper

### Dataset Features

| Feature | Description |
|---|---|
| TV | Advertising expenditure on TV |
| Radio | Advertising expenditure on Radio |
| Newspaper | Advertising expenditure on Newspaper |
| Sales | Product sales (Target Variable) |

## ⚙️ Project Workflow

### 1. Data Collection and Loading

- Imported the Advertising.csv dataset using Pandas.
- Examined the first and last records.
- Checked dataset dimensions and column names.
- Inspected data types and statistical summaries.

### 2. Data Cleaning

- Checked for missing values.
- Identified duplicate records.
- Checked for unwanted index columns.
- Verified the dataset after cleaning.

**Data Cleaning Results:**
- Missing Values: 0
- Duplicate Records: 0

### 3. Exploratory Data Analysis (EDA)

Performed exploratory analysis to understand the distribution of sales and advertising expenditure.

The analysis included:

- Sales distribution using a histogram.
- Statistical summary of advertising variables.
- Unique value analysis.
- Boxplots to examine variable distributions.
- Pairplot to visualize relationships between variables.

### 4. Data Visualization

Created visualizations to understand how advertising expenditure relates to sales.

**TV vs Sales**
- Examined the relationship between TV advertising and product sales.

**Radio vs Sales**
- Analyzed the relationship between Radio advertising and product sales.

**Newspaper vs Sales**
- Investigated the relationship between Newspaper advertising and product sales.

### 5. Correlation Analysis

Calculated the correlation matrix to identify relationships between advertising channels and sales.

Correlation with Sales:

| Feature | Correlation |
|---|---:|
| TV | 0.7822 |
| Radio | 0.5762 |
| Newspaper | 0.2283 |

**Observation:** TV advertising showed the strongest positive correlation with sales among the three advertising channels.

### 6. Feature and Target Selection

Selected the independent and dependent variables.

**Independent Variables (X):**
- TV
- Radio
- Newspaper

**Dependent Variable (y):**
- Sales

### 7. Train-Test Split

Split the dataset into training and testing sets using Scikit-learn.

- Training Data: 80% (160 records)
- Testing Data: 20% (40 records)
- Random State: 42

### 8. Machine Learning Model Development

Implemented two regression algorithms.

**Model 1: Linear Regression**

Linear Regression was used to establish a baseline relationship between advertising expenditure and sales.

The model learns the relationship between the three advertising features and the target sales variable.

**Model 2: Polynomial Regression**

Polynomial Regression was implemented using Scikit-learn's PolynomialFeatures and LinearRegression.

- Polynomial Degree: 2
- Include Bias: False
- Implemented using a Scikit-learn Pipeline.

This model captures nonlinear relationships through polynomial combinations of the input features.

### 9. Model Evaluation

Evaluated both regression models using the following metrics:

- **MAE (Mean Absolute Error):** Measures the average absolute difference between actual and predicted sales.
- **MSE (Mean Squared Error):** Measures the average squared prediction error.
- **RMSE (Root Mean Squared Error):** Measures prediction error in the original target scale.
- **R² Score:** Measures how much variation in sales is explained by the model.

## 📊 Model Performance Comparison

The following results were obtained from the test dataset:

| Evaluation Metric | Linear Regression | Polynomial Regression |
|---|---:|---:|
| MAE | 1.4608 | 0.5262 |
| MSE | 3.1741 | 0.4129 |
| RMSE | 1.7816 | 0.6426 |
| R² Score | 0.8994 | 0.9869 |

### 🏆 Best Performing Model

**Polynomial Regression (Degree 2)**

Based on the evaluation results, Polynomial Regression achieved better performance than Linear Regression.

Key observations:

- Achieved an R² score of 0.9869.
- Achieved an MAE of 0.5262.
- Achieved an RMSE of 0.6426.
- Produced lower prediction errors compared with Linear Regression.

Therefore, Polynomial Regression was selected as the better-performing model for this dataset.

## 📈 Project Visualizations

The notebook includes the following visualizations:

1. Sales Distribution Histogram.
2. TV Advertising vs Sales Scatter Plot.
3. Radio Advertising vs Sales Scatter Plot.
4. Newspaper Advertising vs Sales Scatter Plot.
5. Advertising and Sales Boxplots.
6. Pairplot of Dataset Features.
7. Correlation Heatmap.
8. R² Score Comparison.
9. Actual vs Predicted Sales – Linear Regression.
10. Actual vs Predicted Sales – Polynomial Regression.


## 💡 Skills Demonstrated

- Python Programming
- Data Cleaning and Preprocessing
- Exploratory Data Analysis (EDA)
- Statistical Analysis
- Data Visualization
- Correlation Analysis
- Linear Regression
- Polynomial Regression
- Machine Learning
- Model Evaluation
- Prediction Analysis

## 🏁 Conclusion

This project demonstrates the application of Machine Learning regression techniques to predict product sales using advertising expenditure across TV, Radio, and Newspaper channels.

After performing data cleaning, exploratory data analysis, visualization, and correlation analysis, two regression models were developed and evaluated.

TV advertising showed the strongest positive correlation with sales, with a correlation coefficient of 0.7822.

Among the two models, Polynomial Regression achieved better results, with an R² score of 0.9869, MAE of 0.5262, and RMSE of 0.6426.

The project provided practical experience in regression modelling, data visualization, statistical analysis, and Machine Learning model evaluation.
