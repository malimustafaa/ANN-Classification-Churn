# ANN-Classification-Churn

# Sentiment Analysis with Simple RNN (IMDB Dataset)

This project implements a sentiment classification model using a Simple RNN on the IMDB movie reviews dataset.

## 📘 Dataset
- Source: `tensorflow.keras.datasets.imdb`
- Task: Binary sentiment classification (positive/negative)
- Vocabulary size: 10,000 most frequent words

## 🧠 Model Overview
- **Embedding Layer**: Maps word indices to dense vectors
- **SimpleRNN Layer**: Captures sequential dependencies
- **Dense Layer**: Sigmoid activation for binary classification

## ⚙️ Training
- Loss: `binary_crossentropy`
- Optimizer: `Adam`
- Metrics: `accuracy`

## 📌 Requirements
- TensorFlow
- NumPy

  👤 Author
malimustafaa

## 🔍 Example Code Snippet
```python
model = Sequential()
model.add(Embedding(max_features, 128, input_length=maxlen))
model.add(SimpleRNN(128, activation='relu'))
model.add(Dense(1, activation='sigmoid'))


