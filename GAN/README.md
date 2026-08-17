# GAN Face Generation

A basic Generative Adversarial Network (GAN) built using PyTorch to generate synthetic face images from random noise.

## Problem Statement
The goal is to generate realistic synthetic human face images using a Generative Adversarial Network. The model learns entirely from the CelebA dataset, without any labels, by training two competing networks against each other.

## About the Model
The model consists of two networks:
- **Generator** – Generates fake face images from random noise.
- **Discriminator** – Distinguishes between real CelebA images and generated images.

Both networks are trained together so that the Generator gradually learns to create more realistic face images.

## Data Preprocessing
- Dataset: CelebA Dataset
- Images resized to `64x64`
- RGB images
- Pixel values normalized to `[-1, 1]`

## GAN Architecture
```
Random Noise
        |
        v
Generator
        |
        v
Fake Face
        |
        v
Discriminator
        |
        v
Real / Fake
```
The Generator takes random noise as input and upsamples it into a full RGB face image. The Discriminator takes both real and generated images and predicts whether each one is real or fake. The two networks are trained adversarially, with the Generator improving as it learns to fool the Discriminator.

## Training
- Framework: PyTorch
- Dataset: CelebA
- Optimizer: Adam (Generator and Discriminator)
- Loss Function: Binary Cross-Entropy Loss

## Result
The Generator produces synthetic face images that increasingly resemble real human faces as training progresses.

## Technologies Used
`Python` · `PyTorch` · `Torchvision` · `NumPy` · `Matplotlib` · `Pillow` · `Hugging Face Hub` · `CUDA`
