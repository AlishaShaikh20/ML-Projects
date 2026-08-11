# RNN for IMDB Sentiment Analysis

A Deep Learning project that performs Sentiment Analysis on movie reviews using a Recurrent Neural Network (RNN) built with PyTorch. The model classifies movie reviews as Positive or Negative.

## Project Overview
Sentiment Analysis is a Natural Language Processing (NLP) task that determines the sentiment expressed in text. In this project, movie reviews from the IMDB dataset are preprocessed and converted into numerical representations using TF-IDF. These features are then used to train an RNN-based binary classification model in PyTorch.

## Technologies Used
- Python
- PyTorch
- Pandas
- NumPy
- Scikit-learn
- NLP Preprocessing Techniques

## Dataset
Dataset: IMDB Movie Reviews Dataset

The dataset contains movie reviews labelled as:
- Positive
- Negative

The dataset is not included in this repository because of its large file size.

## Workflow

**1. Data Loading**
- Load the IMDB review dataset using Pandas.

**2. Text Preprocessing**
- Clean and preprocess the review text.
- Prepare the text for numerical representation.

**3. TF-IDF Vectorization**
- Convert textual reviews into numerical feature vectors.
- Limit the feature space to 5,000 features using `TfidfVectorizer`.

**4. Train-Test Split**
- Split the dataset into training and testing sets.
- Test size: 20%
- Random state: 42

**5. Dataset and DataLoaders**
- Convert the processed data into PyTorch tensors.
- Create `TensorDataset` and `DataLoader` objects for training and evaluation.

**6. RNN Model**
The model consists of:
- Recurrent Neural Network (RNN) layer
- Fully Connected layer
- Sigmoid activation for binary classification

- Hidden Size: 128
- RNN Layers: 1
- Optimizer: Adam
- Epochs: 10
- Batch Size: 64

## Model Architecture
```
Input Movie Review
        |
Text Preprocessing
        |
TF-IDF Vectorization
        |
5,000 Features
        |
RNN Layer
(Hidden Size = 128)
        |
Fully Connected Layer
        |
Sigmoid
        |
Positive / Negative
```

## Model Evaluation
The model was evaluated on the test dataset using classification accuracy.

**Final Test Accuracy: 82.85%**

## Project Structure
```
RNN_for_sentiment_analysis/
│
├── rnn_for__sentiment_analysis.ipynb
└── README.md
```

## Future Improvements
- Replace Simple RNN with LSTM
- Experiment with GRU architecture
- Use pretrained word embeddings such as Word2Vec or GloVe
- Implement an Attention Mechanism
- Build a Streamlit web application
- Deploy the model using Flask or FastAPI

## Learning Outcomes
Through this project, I learned:
- Fundamentals of Recurrent Neural Networks
- NLP preprocessing techniques
- TF-IDF text vectorization
- Sequence modeling concepts
- PyTorch model development
- Training and evaluation of deep learning models
- Working with PyTorch `Dataset` and `DataLoader`
