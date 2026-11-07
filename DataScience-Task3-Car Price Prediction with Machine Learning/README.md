# 🚗 Car Price Prediction with Machine Learning

<p align="center">
  <b>Oasis Infobyte – Data Science Internship | Task 3</b>
</p>

## 📌 Project Overview

Car Price Prediction is a Machine Learning project developed to predict the selling price of used cars based on various features such as manufacturing year, present price, kilometers driven, fuel type, seller type, and transmission.

This project uses regression algorithms to analyze historical car data, identify important pricing factors, and predict the estimated selling price of a used vehicle.

The primary objective is to build and evaluate Machine Learning models and identify the best-performing model for used-car price prediction.

## 🎯 Project Objectives

- Analyze used-car data to understand pricing patterns.
- Perform data cleaning and preprocessing.
- Conduct Exploratory Data Analysis (EDA).
- Engineer useful features such as car age and brand.
- Apply regression algorithms for price prediction.
- Evaluate model performance using regression metrics.
- Identify important features influencing car prices.
- Compare actual and predicted selling prices.

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

**Dataset:** CAR DETAILS FROM CAR DEKHO.csv

The dataset contains information about used cars, including their selling prices and vehicle characteristics.

**Important Features:**

| Feature | Description |
|---|---|
| Car_Name | Name of the car |
| Year | Manufacturing year |
| Selling_Price | Selling price of the car (Target Variable) |
| Present_Price | Current showroom price |
| Kms_Driven | Total kilometers driven |
| Fuel_Type | Fuel type of the vehicle |
| Seller_Type | Individual or dealer |
| Transmission | Manual or automatic |
| Owner | Number of previous owners |

## ⚙️ Project Workflow

### 1. Data Collection and Loading
- Imported the dataset using Pandas.
- Inspected dataset dimensions and column information.
- Examined the first few records.

### 2. Data Cleaning and Preprocessing
- Standardized column names.
- Removed duplicate records.
- Normalized categorical values.
- Converted numerical columns into appropriate data types.
- Removed records with missing target values.
- Prepared the dataset for Machine Learning.

### 3. Feature Engineering
Created additional features to improve the prediction process:

- **Car Age:** Calculated using the manufacturing year and current year.
- **Brand:** Extracted the first word from the car name.

### 4. Exploratory Data Analysis (EDA)

Performed different analyses to understand the dataset:

- Distribution of selling prices.
- Selling price comparison by fuel type.
- Relationship between car age and selling price.
- Relationship between kilometers driven and selling price.
- Correlation analysis using a heatmap.

### 5. Feature Preparation and Encoding

- Separated independent variables and the target variable.
- Identified numerical and categorical features.
- Applied median imputation for numerical features.
- Applied most-frequent imputation for categorical features.
- Used One-Hot Encoding for categorical variables.
- Split the dataset into training and testing sets.

**Train-Test Split:**
- Training Data: 80%
- Testing Data: 20%

### 6. Model Training

Implemented and compared two regression algorithms:

**Linear Regression**
- Used as a baseline regression model.
- Identified linear relationships between input features and selling prices.

**Random Forest Regressor**
- Used an ensemble of decision trees.
- Captured more complex relationships between vehicle features and selling prices.
- Used 300 estimators.

### 7. Model Evaluation

Evaluated both models using the following metrics:

- **MAE (Mean Absolute Error):** Measures the average absolute prediction error.
- **RMSE (Root Mean Squared Error):** Measures prediction error while penalizing larger errors.
- **R² Score:** Measures the proportion of target variance explained by the model.

## 📊 Model Performance Comparison

The following results were obtained from the test dataset:

| Model | MAE | RMSE | R² Score |
|---|---:|---:|---:|
| Random Forest Regressor | 149902.591 | 394761.732 | 0.516 |
| Linear Regression | 212414.776 | 441078.347 | 0.396 |

### 🏆 Best Performing Model

**Random Forest Regressor**

The Random Forest Regressor achieved better performance than Linear Regression based on all three evaluation metrics.

- Lower MAE.
- Lower RMSE.
- Higher R² Score.

Therefore, Random Forest Regressor was selected as the best-performing model among the two algorithms tested.

## 📈 Project Visualizations

The notebook includes the following visualizations:

1. Selling Price Distribution.
2. Selling Price vs Fuel Type.
3. Car Age vs Selling Price.
4. Kilometers Driven vs Selling Price.
5. Correlation Heatmap.
6. Actual vs Predicted Selling Prices.
7. Random Forest Feature Importance.

## 🔍 Feature Importance Analysis

Feature importance was analyzed using the best-performing model to understand which variables contribute most to predicting used-car selling prices.

The analysis helps identify the vehicle characteristics that have a stronger influence on the model's predictions.


## 💡 Skills Demonstrated

- Python Programming
- Data Cleaning and Preprocessing
- Exploratory Data Analysis (EDA)
- Feature Engineering
- Data Visualization
- Regression Analysis
- Machine Learning Pipelines
- One-Hot Encoding
- Model Evaluation
- Feature Importance Analysis

## 🏁 Conclusion

This project demonstrates how Machine Learning regression algorithms can be used to predict the selling prices of used cars.

Through data preprocessing, exploratory analysis, feature engineering, and model evaluation, two regression algorithms were developed and compared.

The Random Forest Regressor achieved better results than Linear Regression, with an R² score of 0.516 on the test dataset.

This project provided practical experience in building Machine Learning pipelines, evaluating regression models, and interpreting model performance.
