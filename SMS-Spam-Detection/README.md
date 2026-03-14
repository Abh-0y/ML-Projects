# Overview

This project builds a machine learning based SMS spam detection system that classifies messages as spam or ham (legitimate). With the increase in digital communication, spam messages are widely used for advertising, phishing, and fraud. The goal of this project is to develop an intelligent system that can automatically detect spam messages and help users avoid unwanted or fraudulent communication.
The project applies several machine learning algorithms and ensemble techniques to identify the most effective model for spam detection.

---

# Dataset

The dataset used in this project is the **SMS Spam Collection Dataset** obtained from Kaggle.
- Total messages: 5,574
- Ham messages: 4,516 (87.37%)
- Spam messages: 653 (12.63%)
  
Each record contains:
- v1 → Label (ham or spam)
- v2 → Raw SMS message
  
Since the dataset is highly imbalanced, precision is prioritized over accuracy to reduce false positive predictions.

---

# Text Preprocessing

Before training the models, the text data is cleaned and normalized using several preprocessing steps:
- Convert text to lowercase
- Remove punctuation and special characters
- Remove stopwords
- Lemmatization using WordNetLemmatizer
- Tokenization of text
- Convert processed words back to clean text

These steps help reduce noise and improve model performance.

---

# Exploratory Data Analysis (EDA)

Several analyses were performed to understand the dataset:
- Spam vs Ham distribution
- Character, word, and sentence statistics
- Correlation between text features
- Most common words in spam and Ham messages
- Word cloud visualization

observation: - Spam messages tend to be longer and contain more words and sentences compared to ham messages.

---

# Machine Learning Models

Several machine learning models were implemented and compared:
- Support Vector Machine (LinearSVC)
- Multinomial Naive Bayes
- Logistic Regression
- Random Forest Classifier
- Extra Trees Classifier
- XGBoost Classifier
- Stacking Classifier
- Voting Classifier
Hyperparameter tuning was performed using GridSearchCV.

---

# Evaluation Metrics

Because the dataset is imbalanced, the main focus is on:
- Precision
- Accuracy
Precision is prioritized to reduce false positives, ensuring that legitimate messages are not incorrectly classified as spam.

---

# Best Model
The best performance was achieved using a Voting Classifier, combining:
- Support Vector Machine
- Extra Trees Classifier
- Random Forest Classifier
**Performance:**
- Precision: 1.00
- Accuracy: ~0.976

---

# Tech Stack
•	Python
•	Pandas
•	NumPy
•	Matplotlib
•	Seaborn
•	NLTK
•	Scikit-learn
•	XGBoost
•	WordCloud

