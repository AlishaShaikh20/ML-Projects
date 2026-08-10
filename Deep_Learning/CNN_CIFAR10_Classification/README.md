# CNN – CIFAR-10 Image Classification

This project implements a Convolutional Neural Network (CNN) using PyTorch to classify images from the CIFAR-10 dataset.

## Overview
The model is trained to classify RGB images into one of 10 different categories. The project covers the basic CNN workflow, including:
- Loading the CIFAR-10 dataset
- Image preprocessing and normalization
- Creating training and testing DataLoaders
- Building a CNN architecture using PyTorch
- Training the model using backpropagation
- Evaluating the model on the test dataset
- Calculating classification accuracy

## Dataset
The project uses the CIFAR-10 dataset, which contains:
- 50,000 training images
- 10,000 test images
- Image size: 32 x 32
- Image channels: 3 (RGB)
- 10 classes

The images belong to the following categories:
`airplane`, `automobile`, `bird`, `cat`, `deer`, `dog`, `frog`, `horse`, `ship`, `truck`

## CNN Architecture
The model consists of three convolutional blocks followed by fully connected layers.

```
Input Image
3 x 32 x 32
      |
Conv2D (3 -> 32)
      |
ReLU
      |
MaxPool
      |
Conv2D (32 -> 64)
      |
ReLU
      |
MaxPool
      |
Conv2D (64 -> 128)
      |
ReLU
      |
MaxPool
      |
Flatten
      |
Fully Connected (2048 -> 256)
      |
ReLU
      |
Fully Connected (256 -> 10)
      |
Class Prediction
```

## Preprocessing
The images are converted into PyTorch tensors and normalized before being passed to the model.

```python
transforms.Compose([
    transforms.ToTensor(),
    transforms.Normalize(
        (0.5, 0.5, 0.5),
        (0.5, 0.5, 0.5)
    )
])
```

## Technologies Used
- Python
- PyTorch
- Torchvision
- NumPy
- Jupyter Notebook

## Training
The model is trained using mini-batches through PyTorch's `DataLoader`. The training process includes:
1. Forward propagation
2. Loss calculation
3. Backpropagation
4. Optimizer step

The model is then evaluated using the CIFAR-10 test dataset without calculating gradients.

## Evaluation
Model performance is evaluated using classification accuracy:

```
Accuracy = Correct Predictions / Total Predictions x 100
```

The final test accuracy is calculated after evaluating the model on the complete test dataset. It is 74.71%



## Learning Objectives
This project was created to understand the fundamentals of:
- Convolutional layers
- Pooling layers
- Activation functions
- Flattening CNN feature maps
- Fully connected layers
- Batch processing
- Backpropagation
- Model evaluation using PyTorch

## Reference
This project is part of my Deep Learning learning journey and focuses on implementing a basic CNN from scratch using PyTorch.
