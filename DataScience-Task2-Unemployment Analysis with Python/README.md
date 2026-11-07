# 📊 Unemployment Analysis with Python

<p align="center">
  <b>Oasis Infobyte Data Science Internship – Task 2</b>
</p>

## 📌 Project Overview

This project focuses on analyzing unemployment trends in India using Python and Data Science techniques. The objective is to explore unemployment patterns across different regions, identify monthly variations, compare regional unemployment rates, and investigate changes during the COVID-19 lockdown period.

Using Exploratory Data Analysis (EDA) and data visualization, this project provides insights into India's unemployment situation during the period covered by the dataset.

## 🎯 Objectives

- Analyze unemployment rates across different regions of India.
- Identify monthly unemployment trends and fluctuations.
- Compare unemployment rates across selected states.
- Identify the top 10 regions with the highest average unemployment rates.
- Examine correlations between unemployment, employment, and labour force participation.
- Compare unemployment levels before and during the COVID-19 lockdown period.

## 🛠️ Technologies & Tools Used

| Technology | Purpose |
|---|---|
| Python | Programming language |
| Pandas | Data manipulation and analysis |
| NumPy | Numerical computations |
| Matplotlib | Data visualization |
| Seaborn | Statistical visualization |
| Google Colab | Development environment |

## 📂 Dataset Information

The project uses an Unemployment in India dataset containing information about unemployment rates, estimated employment, and labour force participation across different regions.

**Dataset Details:**
- Total Records Analyzed: 267
- Number of Regions: 27
- Time Period: January 2020 – October 2020

**Key Features:**
- `Region` – Name of the Indian state or region.
- `Date` – Date of observation.
- `Estimated Unemployment Rate (%)` – Estimated unemployment percentage.
- `Estimated Employed` – Estimated number of employed people.
- `Estimated Labour Participation Rate (%)` – Estimated labour force participation percentage.

## ⚙️ Project Workflow

### 1. Data Collection and Loading
- Imported the dataset using Pandas.
- Inspected the dataset structure, columns, and statistical summary.

### 2. Data Cleaning and Preprocessing
- Removed unnecessary spaces from column names and text values.
- Converted date columns into datetime format.
- Converted numerical columns into appropriate data types.
- Removed duplicate records.
- Handled missing values.

### 3. Exploratory Data Analysis (EDA)

Performed the following analyses:

**Regional Unemployment Analysis**
- Calculated the average unemployment rate for each region.
- Compared unemployment rates using horizontal bar charts.

**Monthly Unemployment Trends**
- Analyzed monthly average unemployment rates.
- Visualized unemployment fluctuations using time-series line charts.

**State-wise Comparison**
- Compared unemployment trends across Tamil Nadu, Maharashtra, and Haryana (or other available regions if needed).

**Top 10 Regions Analysis**
- Identified and visualized the ten regions with the highest average unemployment rates.

**Correlation Analysis**
- Examined relationships between unemployment rate, estimated employment, and labour force participation.
- Visualized correlations using a heatmap.

### 4. COVID-19 Impact Analysis

Compared unemployment levels across two periods:

- **Pre-COVID:** Before 25 March 2020.
- **COVID/Lockdown Period:** From 25 March 2020 onwards.

Calculated the average unemployment rate for both periods and analyzed the difference.

### 5. Key Insights
- Identified regions with the highest and lowest average unemployment rates.
- Determined the months with the highest and lowest unemployment averages.
- Analyzed regional and monthly unemployment variations.
- Observed differences in unemployment levels before and during the COVID-19 lockdown period.

## 📈 Key Findings

Based on the dataset analyzed:

| Analysis | Result |
|---|---|
| Highest Unemployment Region | Haryana – 27.48% |
| Lowest Unemployment Region | Meghalaya – 3.87% |
| Highest Unemployment Month | May 2020 – 23.24% |
| Lowest Unemployment Month | October 2020 – 8.03% |
| Pre-COVID Average | 9.23% |
| COVID-Period Average | 12.96% |
| Difference | +3.73 percentage points |

**Important Observation:** The average unemployment rate was higher during the COVID/lockdown period represented in the dataset compared with the pre-COVID period. This comparison shows an association and does not independently establish COVID-19 as the sole cause.

## 📊 Visualizations

The project includes the following visualizations:

1. Average Unemployment Rate by Region.
2. Monthly Average Unemployment Rate in India.
3. Unemployment Rate Comparison Across Three States.
4. Top 10 Regions with Highest Average Unemployment Rates.
5. Correlation Heatmap.
6. Pre-COVID vs COVID-Period Unemployment Comparison.

## 💡 Skills Demonstrated

- Python Programming
- Data Cleaning and Preprocessing
- Exploratory Data Analysis (EDA)
- Statistical Analysis
- Data Visualization
- Time-Series Analysis
- Correlation Analysis
- Data Interpretation

## 🏁 Conclusion

This project provided practical experience in analyzing real-world unemployment data using Python. Through data preprocessing, exploratory analysis, and visualization, unemployment patterns across Indian regions and months were examined.

The COVID-19 period comparison highlighted an increase in average unemployment within the available observations. Overall, this project strengthened my understanding of data analysis, statistical interpretation, and visualization techniques.



