# RNN for IMDB Sentiment Analysis

A Deep Learning project that performs Sentiment Analysis on movie reviews using a Recurrent Neural Network (RNN) built with PyTorch. The model classifies reviews as Positive or Negative based on textual content.

## Project Overview
Sentiment Analysis is a Natural Language Processing (NLP) task that determines the emotional tone behind text. In this project, an RNN model is trained on the IMDB movie review dataset to predict whether a review expresses a positive or negative sentiment.

This project demonstrates:
- Text preprocessing
- Tokenization and vocabulary creation
- Sequence padding
- Dataset and DataLoader creation
- Building an RNN using PyTorch
- Model training and evaluation
- Sentiment prediction

## Technologies Used
- Python
- PyTorch
- Pandas
- NumPy
- Scikit-learn
- NLP Preprocessing Techniques

## Dataset
Dataset: IMDB Movie Reviews Dataset

The dataset contains movie reviews along with sentiment labels:
- Positive
- Negative

The text data is converted into numerical sequences before being fed into the RNN model.

## Workflow

**1. Data Loading**
- Load IMDB review dataset using Pandas.

**2. Text Preprocessing**
- Convert text to lowercase
- Remove unnecessary characters
- Tokenize reviews
- Create vocabulary
- Convert words into integer sequences

**3. Sequence Padding**
- Ensure all review sequences have equal length using padding.

**4. Dataset Preparation**
- Create custom datasets and DataLoaders for efficient batch processing.

**5. RNN Model Architecture**
The model consists of:
- Embedding Layer
- Recurrent Neural Network (RNN) Layer
- Fully Connected Layer
- Sigmoid Activation Function

## Model Architecture
```
Input Text
     |
Tokenization
     |
Word Indexing
     |
Padding
     |
Embedding Layer
     |
RNN Layer
     |
Fully Connected Layer
     |
Sigmoid Output
     |
Positive / Negative
```

Model Evaluation
The model was evaluated using classification accuracy on the test dataset.

Final Test Accuracy: 84.52%

## Project Structure
```
RNN_for_sentiment_analysis/
│
├── rnn_for_sentiment_analysis.ipynb
├── IMDB Dataset.csv
├── README.md
```

## Future Improvements
- Replace Simple RNN with LSTM
- Use GRU architecture
- Apply Pretrained Word Embeddings (Word2Vec/GloVe)
- Implement Attention Mechanism
- Build a Streamlit Web Application
- Deploy the model using Flask/FastAPI

## Learning Outcomes
Through this project, I learned:
- Fundamentals of Recurrent Neural Networks
- NLP preprocessing techniques
- Text vectorization
- Sequence modeling
- PyTorch model development
- Training and evaluation of deep learning models

