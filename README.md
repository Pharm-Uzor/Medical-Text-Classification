# Medical-Text-Classification

## Overview
This repository contains code and data for training a text classification model. The goal of the model is to accurately classify medical findings into one of two determinations 'upheld decision of health plan' or 'overturned decision of health plan' based on their content. Text classification is a common task in natural language processing (NLP) and has applications in sentiment analysis, topic categorization, spam detection, and more.

## Dataset
The dataset used for training and evaluation is the "Independent_Medical_Review__IMR__Determinations__Trend.csv" which is a tabular dataset with multiple columns and rows. The dataset is divided into a training set, a validation set, and a test set. The training set is used to train the model, while the test set is used to evaluate the model's performance on unseen data.

## Model Architecture
The text classification model is based on a Long Short-Term Memory (LSTM) layer, followed by a fully connected dense layer, then the classification head which is a linear dense layer. LSTMs are well-suited for sequential data, such as text, as they can capture contextual information from previous words in the input sequence. LSTM units enhance the model's ability to handle long-range dependencies and mitigate the vanishing gradient problem.

The model takes a sequence of words as input and generates a fixed-length vector representation, which is then passed through the model layers for classification. 
- 'text-classification.ipynb': Script for training the text classification model on the dataset.
- 'Independent_Medical_Review__IMR__Determinations__Trend.csv': Medical text dataset file.

## Training
The dataset was cleaned and prepared for training. The model was trained on the dataset for 15 epochs using a learning rate scheduler.

## Evaluation
The model was evaluated on the test dataset.

## Results
The model's performance on the test set will be displayed. The model performance metric is binary accuracy. 

## Acknowledgments
I would like to acknowledge Prasad Patil for providing the data used in this project.

## Contact
For any inquiries or issues, please contact uzoigodo@gmail.com.
