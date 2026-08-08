# Date Fruit Classification using ANN

This project uses an Artificial Neural Network (ANN) to classify different varieties of date fruits based on their measured features.

## Problem Statement
The goal is to predict the class of a date fruit using machine learning. The dataset contains 34 features related to the size, shape, and other characteristics of date fruits. There are 7 different classes.

## Data Preprocessing
- Features were standardized using `StandardScaler`.
- The target classes were converted into numerical labels using `LabelEncoder`.
- The data was divided into training and testing sets.
- PyTorch `DataLoader` was used to train the model in batches.

## ANN Architecture
```
Input Layer: 34 features
        |
        v
Hidden Layer: 64 neurons + ReLU
        |
        v
Hidden Layer: 64 neurons + ReLU
        |
        v
Output Layer: 7 neurons
```

The output layer has 7 neurons because the dataset contains 7 classes. For each fruit, the model produces 7 output scores, and the class with the highest score is taken as the predicted class.

## Training
- Framework: PyTorch
- Optimizer: Adam
- Loss Function: Cross-Entropy Loss
- Activation: ReLU
- Epochs: 100

## Result
Test Accuracy: 95.0%

The trained ANN achieved 95.0% accuracy on the test dataset.

## Technologies Used
`Python` · `PyTorch` · `Pandas` · `NumPy` · `Scikit-learn`
