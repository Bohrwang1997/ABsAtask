# Aspect-Based Sentiment Analysis (ABSA) Project

This repository contains the implementation of the Aspect-Based Sentiment Analysis (ABSA) task for the CITS4012 Natural Language Processing course project.

## Project Overview

The goal of this project is to identify the sentiment polarity (e.g., positive, negative, neutral) of specific aspects within a given context sentence. For example, given the sentence "great food but the service was dreadful", the sentiment polarities for the aspects "food" and "service" are positive and negative, respectively.

## Dataset

The dataset used in this project is the MAMS dataset, which contains restaurant reviews with multiple aspects and corresponding sentiment polarities. Each instance includes a review, an aspect, and the polarity of that aspect.

### Files Provided
- `train.json`: Training data
- `val.json`: Validation data
- `test.json`: Test data

## Project Structure

The project is implemented in a Jupyter Notebook, which includes the following sections:

### 1. Dataset Processing
General data preprocessing steps are applied, including removing punctuation, eliminating stop words, lemmatizing, converting to lowercase, and expanding contractions. Each model requires a different way of integrating "aspect" information, with specific data preparation steps detailed for each model.

### 2. Model Implementation

#### Model 1: Dual Bi-LSTM Models for Sentence and Aspect
This model employs a Bi-LSTM architecture where both the sentence and aspect are provided as separate inputs to predict polarity.
- **Data Preparation**: Specific steps to prepare the data for this model.
- **Model**: Detailed description and implementation of the model.

#### Model 2: Seq2Seq Model using both Sentence and Aspect
This model uses an encoder-decoder architecture, integrating both the sentence and its associated aspect as input to predict polarity.
- **Data Preparation**: Specific steps to prepare the data for this model.
- **Model**: Detailed description and implementation of the model.

#### Model 3: Fine Tuned Dual Bi-LSTM Models with Attention for Sentence and Aspect
This model employs a Bi-LSTM architecture with an attention mechanism.
- **Data Preparation**: Specific steps to prepare the data for this model.
- **Model**: Detailed description and implementation of the model.

### 3. Testing and Evaluation
This section includes the testing and evaluation of the models. The evaluation metrics and results are provided to compare the performance of the models.

### 4. Object Oriented Programming Codes
This section contains OOP codes relevant to the project.
