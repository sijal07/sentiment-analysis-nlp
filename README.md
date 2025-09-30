# sentiment-analysis-nlp


Sentiment Analysis of Restaurant 
📌 Project Overview

This project applies Natural Language Processing (NLP) and Machine Learning to analyze restaurant reviews and predict whether a review is positive or negative.

The workflow involves:

Data Cleaning – removing special characters, converting text to lowercase, removing stopwords, and applying stemming.

Feature Extraction – converting the cleaned text into numerical format using the Bag of Words model.

Model Training – training a Naive Bayes classifier on the processed data.

Model Testing – splitting the dataset into training and testing sets to evaluate performance.

📂 Dataset

The dataset used is Restaurant_Reviews.tsv.

It contains two columns:

Review → The actual customer review text.

Liked → The sentiment label (1 = positive, 0 = negative).

🔑 Process Explanation
1. Importing Data

The dataset is loaded and prepared for analysis.

2. Text Cleaning & Preprocessing

All non-alphabetical characters are removed.

Text is converted to lowercase for consistency.

Common stopwords like "the", "is", "and" are removed, but the word "not" is kept (since it changes sentiment).

Words are reduced to their root form using stemming (e.g., loved → love).

3. Building the Corpus

Each cleaned review is stored in a list called a corpus, which is later used for feature extraction.

4. Feature Extraction (Bag of Words Model)

The corpus is transformed into a matrix of numbers, where each row represents a review and each column represents the frequency of a particular word.

5. Splitting the Data

The dataset is split into training data (80%) and testing data (20%) to evaluate the model’s performance.

6. Training the Model

A Gaussian Naive Bayes classifier is trained on the training data to learn patterns between words and sentiment labels.

7. Testing the Model

The trained model is tested on unseen data (test set) to check how well it predicts whether reviews are positive or negative.

📊 Results

The model is able to classify restaurant reviews into positive or negative categories.

Accuracy and performance can be evaluated using metrics like accuracy score, confusion matrix, and classification report.
