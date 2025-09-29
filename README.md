# Sentiment Analysis using LSTM

## Project Overview
This project demonstrates text sentiment analysis using Long Short-Term Memory (LSTM) networks in Python. The model classifies customer reviews into positive, negative, or neutral sentiment, showcasing the application of deep learning for natural language processing (NLP) tasks.

## Objective
- To build a robust LSTM model for sentiment classification of textual data.
- To apply preprocessing, tokenization, embedding layers, and LSTM networks to sequence data.
- To evaluate the model using accuracy and loss metrics.

## Dataset
- Source: Publicly available customer reviews dataset (can be Amazon reviews, IMDB dataset, etc.).
- Preprocessing steps:
  - Text cleaning (removal of punctuation, stopwords)
  - Tokenization
  - Padding/truncating sequences for uniform input length
  - Encoding sentiment labels

## Model Architecture
| Layer         | Output Shape | Parameters |
|---------------|-------------|------------|
| Embedding     | (None, 56, 100) | 27,200 |
| LSTM          | (None, 56, 150) | 150,600 |
| LSTM          | (None, 150) | 180,600 |
| Dense         | (None, 272) | 41,072 |
| **Total Params** | 1,198,418 |  |

- Optimizer: Adam
- Loss function: Categorical Crossentropy
- Training epochs: 100
- Batch size: (your batch size)

## Results
- Final training accuracy: **94.65%**
- Final loss: **0.1598**
- Model shows strong capability in classifying textual sentiments accurately.
- Can be extended for real-world applications in customer feedback analysis, social media monitoring, and business intelligence insights.

## Tools & Libraries
- Python, TensorFlow, Keras, NumPy, Pandas
- NLTK / spaCy for text preprocessing
- Matplotlib / Seaborn for visualizations
- Google Colab / Jupyter Notebook for experimentation

