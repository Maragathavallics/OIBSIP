# 📧 Email Spam Detection with Machine Learning

<p align="center">
  <b>Oasis Infobyte – Data Science Internship | Task 4</b>
</p>

## 📌 Project Overview

Email Spam Detection is a Machine Learning and Natural Language Processing (NLP) project developed to classify text messages into two categories: **Spam** and **Ham (Legitimate Messages)**.

The project uses text preprocessing techniques, TF-IDF feature extraction, and supervised Machine Learning algorithms to identify unwanted messages.

Two classification algorithms, Multinomial Naive Bayes and Logistic Regression, are implemented and compared to determine which model performs better in detecting spam messages.

The primary objective is to develop an effective text classification system that can distinguish spam messages from legitimate communication.

## 🎯 Project Objectives

- Understand and analyze the SMS Spam Collection dataset.
- Perform text cleaning and preprocessing using NLP.
- Convert text messages into numerical features using TF-IDF.
- Implement multiple Machine Learning classification algorithms.
- Evaluate model performance using classification metrics.
- Compare the performance of different classification models.
- Visualize spam and legitimate message patterns.
- Test the trained models using new custom messages.
- Save and reload trained models for future predictions.

## 🛠️ Technologies & Libraries Used

| Technology | Purpose |
|---|---|
| Python | Programming language |
| Pandas | Data manipulation |
| NumPy | Numerical computations |
| Matplotlib | Data visualization |
| Seaborn | Statistical visualization |
| NLTK | Natural Language Processing |
| Scikit-learn | Machine Learning |
| WordCloud | Text visualization |
| Joblib | Model serialization |
| Google Colab | Development environment |

## 📂 Dataset Information

**Dataset:** UCI SMS Spam Collection

The dataset contains SMS messages labeled as either spam or ham.

**Dataset Features:**

| Feature | Description |
|---|---|
| label | Message category (spam or ham) |
| message | Original text message |

**Target Variable:** `label`

- `spam` – Unwanted or promotional messages.
- `ham` – Legitimate messages.

## ⚙️ Project Workflow

### 1. Data Collection and Loading

- Downloaded the SMS Spam Collection dataset from the UCI repository.
- Loaded the dataset using Pandas.
- Assigned appropriate column names.
- Inspected the dataset structure and sample records.

### 2. Data Exploration and Cleaning

- Examined dataset dimensions and data types.
- Checked for missing values.
- Identified duplicate messages.
- Removed duplicate and missing records.
- Reset the dataset index.

### 3. Class Distribution Analysis

- Analyzed the distribution of spam and ham messages.
- Calculated class percentages.
- Visualized the distribution using Seaborn count plots.

### 4. Text Preprocessing using NLP

Applied the following Natural Language Processing techniques:

- **Lowercase Conversion:** Converted all text into lowercase.
- **URL Removal:** Removed website links.
- **Email Removal:** Removed email addresses.
- **Punctuation and Number Removal:** Removed unwanted characters.
- **Stopword Removal:** Removed common English words while preserving important negation words.
- **Stemming:** Used Porter Stemmer to reduce words to their root forms.

A custom text preprocessing function was developed to clean the messages.

### 5. TF-IDF Feature Extraction

Implemented TF-IDF (Term Frequency–Inverse Document Frequency) to convert text messages into numerical representations.

Configuration:
- Maximum Features: 5,000
- N-gram Range: (1, 2)
- Minimum Document Frequency: 2
- Sublinear TF: Enabled

TF-IDF helps identify important words and phrases for spam classification.

### 6. Train-Test Split

Divided the dataset into training and testing sets.

- Training Data: 80%
- Testing Data: 20%
- Random State: 42
- Stratification: Enabled

### 7. Machine Learning Model Training

Implemented two supervised classification algorithms.

**Model 1 – Multinomial Naive Bayes**

- Uses probability-based classification.
- Suitable for text classification problems.
- Predicts whether a message belongs to spam or ham.

**Model 2 – Logistic Regression**

- Uses a logistic function for binary classification.
- Configured with a maximum of 1,000 iterations.
- Used balanced class weights to address class imbalance.

### 8. Model Evaluation

Evaluated both models using:

- **Accuracy:** Overall percentage of correct predictions.
- **Precision:** Percentage of predicted spam messages that were actually spam.
- **Recall:** Percentage of actual spam messages correctly identified.
- **F1-Score:** Harmonic mean of precision and recall.
- **Confusion Matrix:** Visualizes correct and incorrect classifications.

### 9. Model Comparison

Compared both algorithms using a performance metrics table and bar chart.

### 10. WordCloud Visualization

Generated separate WordCloud visualizations for:

- Spam Messages.
- Ham Messages.

These visualizations help identify frequently occurring words in each message category.

### 11. Custom Message Prediction

Developed a custom prediction function that:

1. Accepts a new text message.
2. Applies NLP preprocessing.
3. Converts the message using the trained TF-IDF vectorizer.
4. Predicts the result using both trained models.
5. Displays the classification as SPAM or HAM.

### 12. Model Saving and Loading

Used Joblib to save and reload the trained models and TF-IDF vectorizer.

Saved files:

- `spam_nb_model.pkl`
- `spam_lr_model.pkl`
- `tfidf_vectorizer.pkl`

This allows the trained models to be reused without retraining.

## 📊 Model Performance Comparison

The following results were obtained from the test dataset:

| Evaluation Metric | Multinomial Naive Bayes | Logistic Regression |
|---|---:|---:|
| Accuracy | 96.62% | 96.81% |
| Precision | 98.98% | 84.03% |
| Recall | 74.05% | 92.37% |
| F1-Score | 84.72% | 88.00% |

### 🏆 Best Performing Model

**Logistic Regression**

Based on the evaluation results, Logistic Regression achieved better overall performance.

Key observations:

- Achieved 96.81% accuracy.
- Achieved 92.37% recall.
- Achieved an 88.00% F1-score.
- Identified 121 out of 131 actual spam messages correctly.

Although Multinomial Naive Bayes achieved higher precision (98.98%), Logistic Regression achieved better recall and F1-score.

Therefore, Logistic Regression was selected as the better overall model for this project, particularly when detecting as many spam messages as possible is important.

## 📈 Project Visualizations

The project includes the following visualizations:

1. Spam vs Ham Message Distribution.
2. Model Performance Comparison.
3. Multinomial Naive Bayes Confusion Matrix.
4. Logistic Regression Confusion Matrix.
5. Spam Messages WordCloud.
6. Ham Messages WordCloud.


## 💡 Skills Demonstrated

- Python Programming
- Natural Language Processing (NLP)
- Text Preprocessing
- TF-IDF Vectorization
- Exploratory Data Analysis
- Data Visualization
- Text Classification
- Multinomial Naive Bayes
- Logistic Regression
- Model Evaluation
- Confusion Matrix Analysis
- Model Serialization using Joblib

## 🔮 Future Enhancements

- Implement Support Vector Machine (SVM).
- Experiment with advanced NLP techniques.
- Explore deep learning models such as LSTM.
- Train using larger real-world email datasets.
- Develop an interactive web application using Streamlit.
- Integrate real-time email spam classification.

## 🏁 Conclusion

The Email Spam Detection project was successfully implemented using Natural Language Processing and Machine Learning techniques.

Text preprocessing and TF-IDF feature extraction were used to transform raw messages into meaningful numerical representations. Two classification algorithms, Multinomial Naive Bayes and Logistic Regression, were trained and evaluated.

Logistic Regression achieved the best overall performance with an accuracy of 96.81%, recall of 92.37%, and F1-score of 88.00%.

The project demonstrates how NLP and Machine Learning can be combined to build an effective spam classification system.
