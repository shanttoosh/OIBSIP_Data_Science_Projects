# Twitter Sentiment Analysis

## Introduction

As part of my internship at Oasis Infobyte, I successfully completed my fifth task: This project involves analyzing tweets related to various airlines to determine the sentiment of the tweets. The dataset contains tweets labeled as positive, negative, or neutral. The goal of the project is to clean and preprocess the text data, perform exploratory data analysis (EDA), and build machine learning models to classify the sentiment of the tweets.

## Table of Contents
1. [Data Loading & Initial Exploration](#data-loading--initial-exploration)
2. [Text Preprocessing](#text-preprocessing)
3. [Data Cleaning](#data-cleaning)
4. [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
5. [Feature Engineering](#feature-engineering)
6. [Model Training & Evaluation](#model-training--evaluation)
7. [Visualization](#visualization)

## Data Loading & Initial Exploration

- The dataset `Tweets.csv` is loaded, and initial exploration is performed to understand the structure of the data and identify the unique sentiment values present in the dataset.

## Text Preprocessing

- A function `clean_the_tweet` is used to clean the tweet text by removing non-alphabetic characters, converting text to lowercase, and removing unnecessary tokens.
- Another function `text_process` is utilized to remove punctuation and stopwords to prepare the text data for modeling.

## Data Cleaning

- Neutral sentiments are filtered out from the dataset.
- A new column `cleaned_tweet` is created by applying the `clean_the_tweet` function.
- Sentiment values are converted into binary labels (1 for positive, 0 for negative).
- The cleaned data is saved to an Excel file and reloaded for further processing.

## Exploratory Data Analysis (EDA)

- Various visualizations are created to explore the data:
  - Count plots for sentiment distribution, airline distribution, and user timezones.
  - A box plot is used to identify outliers in the `airline_sentiment_confidence` column.

## Feature Engineering

- The `tweet_created` time is converted into a datetime object, and the hour of the tweet is extracted to create a new feature.

## Model Training & Evaluation

- Functions are defined to handle model training, evaluation, and hyperparameter tuning using grid search.
- Various machine learning models (e.g., Naive Bayes, SVM) are trained on the data, and their performance is evaluated using metrics such as accuracy, ROC-AUC, precision-recall curves, and confusion matrices.

## Visualization

- The relationship between the tweet hour and sentiment is visualized using count plots to identify any patterns in sentiment based on the time of the tweet.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Connect with Me

Feel free to connect with me on [LinkedIn](https://www.linkedin.com/in/shanttoosh-v-470484289/) and follow my journey in data analytics and visualization!


