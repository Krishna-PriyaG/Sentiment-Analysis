# Movie Reviews Sentiment Analysis
This project performs sentiment analysis on the IMDb movie reviews dataset using different machine learning models and feature extraction techniques. The goal is to classify movie reviews as either positive or negative.

## Table of Contents
- Dataset
- Data Preprocessing
- Feature Extraction
- Model Training and Evaluation
- Results
- Visualizations
- Requirements
- Usage

## Dataset
The dataset used is the IMDb movie reviews dataset from the NLTK corpus. It consists of 2000 movie reviews, evenly split between positive and negative sentiments.

## Data Preprocessing
- Tokenization: Split the reviews into individual words.
- Stopword Removal: Remove common English stopwords.
- Lemmatization: Reduce words to their base or root form.

## Feature Extraction
Two feature extraction techniques are used:
- Term Frequency (TF): Counts the frequency of words in the document.
- Term Frequency-Inverse Document Frequency (TF-IDF): Adjusts the frequency of words by how often they appear in all documents.

## Model Training and Evaluation
Three classifiers are trained and evaluated:
- Naive Bayes (MultinomialNB)
- Logistic Regression
- Multi-layer Perceptron (MLP)
  
Each classifier is evaluated using both TF and TF-IDF feature representations. The performance is measured using accuracy, True Positive Rate (TPR), and False Positive Rate (FPR). Confusion matrices are also displayed.

## Results 
The accuracy of each model with different feature representations is as follows:

Model	              TF Accuracy	TF-IDF Accuracy
Naive Bayes	        0.83	      0.84
Logistic Regression	0.86	      0.87
MLP               	0.85	      0.86

## Visualizations
A bar chart is used to compare the accuracy of the different models with TF and TF-IDF representations

## Requirements
- Python 3.6+
- NLTK
- scikit-learn
- matplotlib
- numpy
Install the necessary packages using:
```bash
pip install nltk scikit-learn matplotlib numpy
```
## Usage
Download NLTK data files:
```python
import nltk
nltk.download('movie_reviews')
nltk.download('punkt')
nltk.download('stopwords')
nltk.download('wordnet')
```
The script will output the accuracy of each model and display confusion matrices and accuracy comparison charts.

This project provides insights into the effectiveness of different models and feature extraction techniques for sentiment analysis on movie reviews.
