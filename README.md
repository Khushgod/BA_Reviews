✈️British Airways Review Analysis & Sentiment Prediction

📌 Project Overview
This project is a deep dive into the voice of British Airways customers, harnessing the power of Natural Language Processing (NLP) and Machine Learning (ML) to unearth insights from reviews scraped from Skytrax. Our objective? Not just to analyze what customers are saying—but to understand how they feel, what matters to them most, and to build a predictive sentiment classifier that captures these nuances with high accuracy.

📥 Data Collection
Reviews were programmatically scraped from the Skytrax website. Each record includes:
✍️ Customer review text
✅ Verification status

After collection, data underwent rigorous cleaning and structuring to prepare it for downstream analysis.
🧪 Analysis Pipeline


🔧 1. Data Preprocessing
A robust NLP pipeline was developed:
Text cleaning (lowercasing, punctuation & special character removal)
Tokenization and lemmatization
Airline-specific stopword removal
Feature extraction using TF-IDF


📊 2. Exploratory Data Analysis
Comprehensive exploratory analysis was conducted through:
Sentiment Analysis with VADER and TextBlob
Topic Modeling via Latent Dirichlet Allocation (LDA)
Word Clouds per sentiment category
Aspect-Based Sentiment Analysis (crew, food, service, etc.)

🤖 Machine Learning Model
A Logistic Regression model was trained on TF-IDF features to classify review sentiments.
📈 Performance Summary

Test Set Accuracy: 0.8462

Classification Report Highlights:

Sentiment	Precision	Recall	F1-score
Negative	82%	89%	86%
Positive	87%	80%	84%

Macro Avg: 85% Precision | 84% Recall | 85% F1-score

Weighted Avg: 85% across all metrics

💡 Conclusion: Our model reliably captures sentiment nuances with strong predictive performance.

Requirements
Install all required packages using:
pip install pandas numpy matplotlib seaborn nltk scikit-learn wordcloud gensim pyLDAvis textblob joblib
