# Sentiment Analysis with Deep Learning models

This repository contains a Jupyter Notebook implementing sentiment analysis on attraction reviews using Convolutional Neural Networks (CNN) and Bidirectional Long Short-Term Memory (BiLSTM) models. The project preprocesses text data, trains deep learning models, and evaluates their performance using various metrics, including F1-score.

## Project Overview

The notebook performs sentiment analysis on a dataset of attraction reviews, predicting whether a review expresses positive or negative sentiment. The key components include:

- **Data Preprocessing**: Cleaning and preparing text data by handling emojis, contractions, slang, URLs, and special characters, followed by tokenization, stopword removal, and lemmatization.
- **Feature Engineering**: Utilizing GloVe embeddings for word representations and preparing tokenized sequences for model input.
- **Models**: Implementing and comparing four models:
  - CNN-BiLSTM
  - BiLSTM
  - GloVe CNN-BiLSTM
  - GloVe BiLSTM
- **Evaluation**: Assessing model performance using F1-score, classification reports, and confusion matrices.
- **Results**: The CNN-BiLSTM model achieved the highest F1-score of 0.8866.

## Dataset

The dataset used contains reviews of attractions, including the following columns:
- `attraction`: Name of the attraction (e.g., Pyramids of Giza).
- `rate`: Rating given (e.g., 5.0).
- `date`: Review date.
- `review`: Text of the review.
- `sentiment`: Binary sentiment label (0 for negative, 1 for positive).
- Additional columns for processed text and sentiment scores.


## Results

The models were evaluated using the F1-score on a test set of 1169 samples. The results are as follows:

- **CNN-BiLSTM**: F1-score = 0.8866
- **BiLSTM**: F1-score = 0.8739
- **GloVe CNN-BiLSTM**: F1-score = 0.8665
- **GloVe BiLSTM**: F1-score = 0.8757

The **CNN-BiLSTM** model performed the best, achieving an F1-score of **0.8866**. Confusion matrices and classification reports are provided in the notebook for detailed performance analysis.

## Acknowledgments

This project was completed under the guidance of:
- **Teaching Assistant Esraa Taher**, who provided valuable support and feedback.
- **Dr. Ibrahim Zaghloul**, whose expertise were instrumental in the project's success.
