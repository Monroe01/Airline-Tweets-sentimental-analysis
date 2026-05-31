# Airline Tweets Sentiment Analysis

A complete NLP sentiment classification project built on airline-related Twitter data, covering the full machine learning workflow from text preprocessing and exploratory analysis to traditional machine learning, deep learning, and transformer-based models.

This project focuses on understanding how different NLP modeling approaches perform on short-text sentiment classification tasks and compares traditional ML models, recurrent neural networks, and transformer architectures.

---

## Project Overview

The goal of this project is to classify user sentiment from airline-related tweets and systematically compare different NLP approaches under the same dataset and evaluation setting.

The project includes:

- Data cleaning and exploratory data analysis (EDA)
- Text preprocessing and feature engineering
- Traditional machine learning models
- Deep learning sequence models (RNN / LSTM / GRU)
- Transformer-based models (BERT / RoBERTa / DistilRoBERTa)
- Model comparison and evaluation

---

## Dataset

Dataset: Airline Tweets Sentiment Dataset

The dataset contains airline-related Twitter posts labeled by sentiment.

### Target Labels
- Positive
- Neutral
- Negative

### Challenges
- Noisy short text
- Informal language
- Emojis and abbreviations
- Misspellings
- Class imbalance
- Limited contextual information

The project focuses on understanding how NLP models handle real-world noisy social media text.

---

## NLP Pipeline

text id="m5k4tg" Raw Tweets       ↓ Cleaning & EDA       ↓ Text Preprocessing (Tokenization, Lemmatization, Normalization)       ↓ Feature Engineering (TF-IDF / Vocabulary Encoding)       ↓ Traditional ML Models (Logistic Regression / SVM / RF / XGBoost)       ↓ Deep Learning Models (RNN / LSTM / GRU)       ↓ Transformer Models (BERT / DistilRoBERTa / RoBERTa)       ↓ Evaluation & Comparison 

---

## Project Structure

text id="ph39pk" airline-tweets-sentiment-analysis/ │ ├── notebooks/ │   ├── 01_EDA_Preprocessing.ipynb │   ├── 02_Traditional_ML.ipynb │   ├── 03_RNN_LSTM_GRU.ipynb │   └── 04_Transformer_Models.ipynb │ ├── results/ │ ├── requirements.txt └── README.md 

---

## Cleaning & EDA

The project begins with exploratory data analysis and preprocessing to better understand tweet characteristics and improve model performance.

### Preprocessing Steps
- Text normalization
- URL and punctuation removal
- Emoji handling
- Contraction expansion
- Tokenization
- Stopword processing
- Lemmatization
- Tweet cleaning

### EDA
- Sentiment distribution analysis
- Word frequency analysis
- Word cloud visualization
- Tweet length distribution
- Class imbalance inspection

The preprocessing stage was designed to improve robustness when handling noisy social media text.

---

## Traditional Machine Learning Models

Traditional NLP baselines were built using TF-IDF features and compared across multiple classifiers.

### Feature Engineering
- TF-IDF vectorization
- Text normalization
- Vocabulary representation

### Models
- Logistic Regression
- Support Vector Machine (SVM)
- Random Forest
- XGBoost

### Goal
Evaluate how classical NLP approaches perform on short-text sentiment classification before moving to neural architectures.

---

## Deep Learning Models

Sequence-based neural models were implemented to capture contextual dependencies in text.

### Models
- RNN
- LSTM
- GRU

### Implementation Details
- PyTorch implementation
- Vocabulary encoding
- Sequence vectorization
- DataLoader pipeline
- Batch training
- Sequence modeling for tweet sentiment classification

The project explored how recurrent architectures handle short social media text and contextual information.

---

## Transformer Models

Transformer-based language models were fine-tuned and compared for sentiment classification.

### Models
- DistilRoBERTa
- RoBERTa Base
- BERT Base

### Workflow
- Tokenization using pretrained tokenizers
- Fine-tuning pretrained language models
- Sequence truncation and padding
- Classification evaluation

The objective was to understand how pretrained transformer architectures outperform traditional and recurrent approaches in sentiment classification.

---

## Evaluation

Model performance was evaluated using classification metrics and confusion matrices.

### Evaluation Metrics
- Accuracy
- Precision
- Recall
- F1-score
- Classification report
- Confusion matrix

The project compares model performance across:

text id="h2lqwh" Traditional ML vs RNN-based architectures vs Transformer-based models 

to better understand trade-offs between performance, complexity, and representation learning.

---

## Key Findings

### Traditional Models
- Strong baselines for structured short-text classification
- TF-IDF + SVM/Logistic Regression performed competitively

### RNN-Based Models
- Better contextual understanding than traditional models
- Improved sequential representation of tweet content

### Transformer Models
- Achieved the strongest performance overall
- Better semantic understanding and contextual modeling
- More robust to noisy and informal text

The project demonstrates how modern NLP architectures improve performance on sentiment classification tasks.

---

## Tech Stack

### Programming
- Python

### NLP / ML
- Scikit-learn
- PyTorch
- Hugging Face Transformers
- NLTK

### Models
- Logistic Regression
- SVM
- Random Forest
- XGBoost
- RNN
- LSTM
- GRU
- BERT
- DistilRoBERTa
- RoBERTa

### Data Processing
- TF-IDF
- Tokenization
- Lemmatization
- Vocabulary Encoding
- Text Cleaning

### Visualization
- Matplotlib
- WordCloud

---

## What I Learned

Through this project, I gained hands-on experience with:

- End-to-end NLP pipelines
- Text preprocessing for noisy social media data
- Traditional machine learning baselines
- Sequence modeling using RNN/LSTM/GRU
- Fine-tuning transformer models
- Model comparison and evaluation
- Experiment workflow design
- Trade-offs between classical ML and deep learning approaches

This project helped me better understand how NLP systems are built, evaluated, and iteratively improved in real-world sentiment classification tasks.

---

## Future Improvements

Potential future improvements include:

- Hyperparameter tuning
- Better handling of class imbalance
- More advanced preprocessing strategies
- Error analysis and explainability
- Experiment tracking
- Model deployment as an inference API

---

## Motivation

This project was built to explore the evolution of NLP approaches for sentiment classification — from traditional machine learning methods to deep learning and transformer-based architectures.

Rather than focusing on a single model, the project emphasizes experimentation, comparison, and understanding of how different NLP techniques behave on noisy short-text data.
