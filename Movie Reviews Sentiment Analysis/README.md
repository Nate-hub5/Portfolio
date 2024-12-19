# Problem Description:
https://github.com/Nate-hub5/Portfolio/blob/main/Movie%20Reviews%20Sentiment%20Analysis/Movie%20Reviews%20Sentiment%20Analysis.ipynb

This project focuses on sentiment analysis of movie reviews from the IMDB dataset. The goal is to classify movie reviews as either positive or negative using machine learning techniques. The project emphasizes data preprocessing, exploratory data analysis (EDA), text normalization, and experimentation with multiple models to identify the best-performing approach.

# Table of Contents

1. Load and Inspect Data
2. EDA
3. Evaluation Procedure
4. Text Normalization
5. Train / Test Split
6. Model experiments
7. My Reviews
   
# Project Instructions:

**1. Load and Inspect Data**
* Import libraries
* Load the IMDB dataset form a .tsv file.
* Check for missing / duplicated values

**2. EDA**
* Check number of movies and reviews over the years
* Check the distribution of number of reviews per movie
* Distribution of ratings for train and test set
* Number of reviews of different polarities per year

**3. Evaluation Procedure**
* Create a dictionary to store evaluation metrics to loop the train/test set
* Metrics Calculation using Accuracy, F1, APS, and ROC AUC
* Visualizations of metrics

**4. Text Normalization**
* Convert all text in reviews to lowercase
* Remove all digits from text
* Remove all punctuation and special characters

**5. Train / Test Split**
* Dataset already had split data so we needed to seperate them

**6. Model experiments**
* Constant model
* NLTK, TF-IDF and LR model
* SpaCy, TF-IDF and LR model
* SpaCy, TF-IDF and LGBMClassifier

**7. My Reviews**
* Testing my own reviews with the different models
