# Project-2-NLP-Challenge_Group3
📌 Introduction
This repository contains a Natural Language Processing (NLP) project aimed at developing a binary text classifier to distinguish between real and fake news based on article headlines and content. This challenge simulates a real-world task where preprocessing, model selection, and evaluation play a crucial role in building an effective NLP pipeline.

🗂️ Dataset
The main training dataset is located in dataset/data.csv and includes the following columns:

label: Target variable (0 = Fake News, 1 = Real News)

title: News article headline (all in lower case)

Additionally, dataset/validation_data.csv is provided for testing the final model. It contains news samples labeled as 2, which must be replaced with predicted labels (0 or 1) using the trained classifier.

🎯 Objective
Build and evaluate a machine learning model that can accurately predict whether a given news article is real or fake. Your final output should be a new version of validation_data.csv where all label values of 2 are replaced by predictions (0 or 1), preserving the original file structure.

⚙️ Workflow
1. Data Cleaning & Preprocessing
  1.1 Handle missing values
  1.2 Apply text normalization (removing punctuation, stopwords, etc.)

2. Train-Test Split
   2.1 Split data.csv into training and testing subsets.

3. Model Building
   3.1 Implement a pipeline using TF-IDF/BoW... + a classifier model (RandomForest, LogisticRegression...)
   3.2 Train the model on the training set

4. Model Evaluation
   4.1 Evaluate model performance on the test set using classification metrics

5. Prediction on Validation Data
   5.1 Use the trained model to predict labels in validation_data.csv
   5.2 Replace label 2 with predictions, save results to validation_data_predicted.csv

6. Make a prediction on the accuracy our model will get when comparing our predictions with the real results.

7. Prepare a PPT presentation, explaining the styeps we've followed, together with the obtained results. 
