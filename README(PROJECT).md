Spam Detection 
Overview

This project implements a simple spam detection system for email messages using Python. It uses TF-IDF Vectorization for feature extraction and the Multinomial Naive Bayes algorithm for classification. The model predicts whether a given email is spam or not spam.

Features
Preprocesses datasets with different column names (v1, v2, label, message, Category, Message).
Handles missing values.
Converts textual labels into numerical values (ham → 0, spam → 1).
Splits data into training and testing sets (80/20 split).
Uses TF-IDF vectorization for text representation.
Evaluates model performance using accuracy and classification report.
Allows testing of new email messages for spam prediction.
Dataset
The project uses a CSV file containing email messages labeled as ham or spam.
The dataset can have different column names; the code automatically standardizes them to label and message.
Example file path used:
/content/drive/MyDrive/Internship Work/spam.csv
Requirements
Python 3.x
pandas
numpy
scikit-learn

Install required libraries using:

pip install pandas numpy scikit-learn
How to Run
Load the dataset CSV file.
Run the Python script.
The script will:
Preprocess the data.
Train the Naive Bayes model.
Evaluate accuracy and print the classification report.
Test a custom email by updating the email list in the script.
