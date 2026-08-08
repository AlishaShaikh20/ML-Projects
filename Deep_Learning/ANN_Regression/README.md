# Power Plant Energy Output Prediction using Artificial Neural Networks

## Project Overview
This project implements an Artificial Neural Network (ANN) using PyTorch to predict the electrical power output of a Combined Cycle Power Plant based on environmental conditions. The project demonstrates the complete deep learning workflow, from data preprocessing to model evaluation.

## Problem Statement
Predict the net hourly electrical energy output (PE) of a power plant using the following environmental features:
- Ambient Temperature (AT)
- Exhaust Vacuum (V)
- Ambient Pressure (AP)
- Relative Humidity (RH)

This is a regression problem where the goal is to accurately estimate continuous power output values.

## Technologies Used
- Python
- PyTorch
- Pandas
- NumPy
- Matplotlib
- Scikit-learn

## Workflow
- Data preprocessing
- Train-Test Split
- Feature Standardization using StandardScaler
- Conversion to PyTorch Tensors
- DataLoader for mini-batch training
- ANN Model Development
- Model Training using Adam Optimizer
- Validation Loss Monitoring
- Best Model Checkpoint Saving
- Model Evaluation

## Model Architecture
```
Input Layer (4 Features)
        |
        v
Hidden Layer (6 Neurons)
        |
      ReLU
        |
        v
Hidden Layer (6 Neurons)
        |
      ReLU
        |
        v
Output Layer (1 Neuron)
```

## Loss Function
- Mean Squared Error (MSE)

## Optimizer
- Adam Optimizer

## Results
| Metric | Value |
|--------|-------:|
| Training MSE | 19.51 |
| Testing MSE | 17.82 |
| R2 Score | 0.9377 |

The model achieved a high R2 score of 0.9377, indicating excellent predictive performance. The close training and testing MSE values suggest that the model generalizes well to unseen data without significant overfitting.

## Project Files
- `Power_Plant_ANN_Regression.ipynb` - Complete implementation
- `power_plant_dataset.csv` - Dataset
- `best_model.pt` - Saved trained model

## Key Learning Outcomes
- Building Artificial Neural Networks using PyTorch
- Feature standardization for neural networks
- Creating custom ANN architectures
- Forward and backward propagation
- Mini-batch training using DataLoader
- Saving and loading trained models
- Evaluating regression models using MSE and R2 Score
- Visualizing training and validation loss


