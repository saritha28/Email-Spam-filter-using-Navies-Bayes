# Email Spam Filter using Naive Bayes

## Overview
This project implements a spam filter using the Naive Bayes algorithm to classify emails as spam or ham (non-spam). The model is trained on a dataset containing labeled emails and achieves high accuracy in distinguishing between spam and non-spam messages.

## Table of Contents
- [Introduction](#email-spam-filter-using-naive-bayes)
- [Data Description](#data-description)
- [Data Preprocessing](#data-preprocessing)
- [Feature Extraction](#feature-extraction)
- [Naive Bayes Classification](#naive-bayes-classification)
- [Model Evaluation](#model-evaluation)
- [Cross Validation using Pipeline](#cross-validation-using-pipeline)
- [Usage](#usage)

## Data Description
The dataset used contains emails labeled as spam or ham. It includes columns for message content and a categorical column indicating spam or ham.

## Data Preprocessing
- The 'Category' column is converted to binary values (1 for spam, 0 for ham).
- Train-test split is performed to prepare the data for training and testing the model.

## Feature Extraction
- The 'Message' column is converted to numeric form using the CountVectorizer technique.
- CountVectorizer transforms text data into a matrix of word counts to be used as features for the model.

## Naive Bayes Classification
- Multinomial Naive Bayes algorithm is utilized for text classification.
- The model is trained using the transformed feature matrix of the 'Message' column.

## Model Evaluation
- Accuracy is computed using the test dataset, achieving a high accuracy score of approximately 98.42%.
- Predictions are made on sample emails to demonstrate the classifier's functionality.

## Cross Validation using Pipeline
- A pipeline is constructed, including the vectorizer and Naive Bayes classifier.
- The pipeline is fitted to the data and evaluated, showing a consistent accuracy score of approximately 98.42%.

## Usage
- The project can be utilized to classify emails as spam or ham using the provided Naive Bayes classifier.
- Expand the code for experimentation with different preprocessing techniques or models.

