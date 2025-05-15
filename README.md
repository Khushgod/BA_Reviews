British Airways Review Analysis & Sentiment Prediction

Project Overview
This project involves a comprehensive analysis of British Airways customer reviews scraped from Skytrax. Using natural language processing techniques, sentiment analysis, topic modeling, and machine learning approaches, we analyze customer opinions to extract insights and build a predictive model for sentiment classification.

Data Collection
Web scraping was used to collect British Airways reviews from the Skytrax website
Data includes review text and verification status
The scraped data was cleaned and preprocessed to create a structured dataset for analysis

Analysis Pipeline
The project is divided into several key steps:
1. Data Preprocessing

Text cleaning (removing special characters, lowercasing)
Tokenization and lemmatization
Stopword removal with airline-specific custom stopwords
Feature extraction for machine learning

2. Exploratory Data Analysis

Sentiment Analysis: Using VADER and TextBlob to classify reviews as positive, neutral, or negative
Topic Modeling: Applying Latent Dirichlet Allocation (LDA) to discover review themes
Word Cloud Generation: Creating visualizations of most frequent terms overall and by sentiment
Aspect-Based Analysis: Examining sentiment toward specific aspects like crew, food, service, etc.

3. Machine Learning Model
We developed a sentiment prediction model using Logistic Regression:
Model Performance:
Accuracy on test set: 0.8462

Classification Report:
              precision    recall  f1-score   support
   negative       0.82      0.89      0.86       100
   positive       0.87      0.80      0.84        95
   
   accuracy                           0.85       195
  macro avg       0.85      0.84      0.85       195
weighted avg      0.85      0.85      0.85       195
This strong performance (85% accuracy) demonstrates that our model effectively captures sentiment patterns in British Airways reviews.

Key Features
Comprehensive Text Preprocessing: Multi-stage cleaning and normalization pipeline for review text
Multi-faceted Analysis: Combined analysis approaches:

Sentiment scoring and classification
Topic discovery through LDA
Word frequency and association analysis
Aspect-based sentiment extraction


Interactive Visualizations:

Sentiment distribution charts
Topic distribution analysis
Word clouds for different sentiments
Feature importance visualizations


Predictive Modeling:

TF-IDF vectorization of review text
Logistic Regression with hyperparameter tuning
Cross-validation for performance evaluation
Model persistence for future use


Feature Importance Analysis:

Identification of key terms associated with positive/negative sentiment
Understanding the most predictive words for sentiment classification



Installation & Usage

Requirements
pandas
numpy
matplotlib
seaborn
nltk
scikit-learn
wordcloud
gensim (optional, for topic modeling)
pyLDAvis (optional, for topic visualization)
textblob
joblib
