# Vanilla GAN for Face Generation

## Overview

This project implements a Vanilla Generative Adversarial Network (GAN) using PyTorch to generate human face images from random noise vectors.

The model is trained on the CelebA dataset and demonstrates the fundamental working of GANs using fully connected neural networks.

---

## Features

* Built completely from scratch using PyTorch
* Custom dataset loading and preprocessing
* Generator and Discriminator networks
* Real-time generated image visualization
* GPU support using CUDA/MPS
* Beginner-friendly GAN implementation

---

## Tech Stack

* Python
* PyTorch
* Torchvision
* NumPy
* Matplotlib
* PIL

---

## Dataset

Dataset Used: CelebA Dataset

The dataset contains more than 200,000 celebrity face images.

Image preprocessing includes:

* Center Cropping
* Resizing to 64×64
* Tensor Conversion
* Normalization to [-1,1]

---

## Project Structure

```bash
├── gan_training.py
├── README.md
├── generated_images/
├── saved_models/
└── dataset/
```

---

## Generator Architecture

The Generator network converts random noise vectors into fake human face images.

Architecture:

* Linear Layers
* ReLU Activations
* Tanh Output Layer

---

## Discriminator Architecture

The Discriminator network classifies images as:

* Real
* Fake

Architecture:

* Fully Connected Layers
* LeakyReLU Activations
* Sigmoid Output Layer

---

## Training Process

The GAN follows adversarial training:

1. Train the Discriminator on:

   * Real images
   * Fake images

2. Train the Generator to fool the Discriminator

Loss Function:

* Binary Cross Entropy Loss (BCELoss)

Optimizer:

* Adam Optimizer

---


---

## Results

The model gradually learns to generate synthetic celebrity face images from random noise vectors through adversarial learning.

---

## Future Improvements

* Upgrade to DCGAN
* Add Convolutional Layers
* Improve image quality
* Implement Wasserstein GAN (WGAN)
* Add model checkpointing
* Deploy using Streamlit

---

## Learning Outcomes

Through this project, I learned:

* Fundamentals of GANs
* Adversarial training
* Generator vs Discriminator dynamics
* Image preprocessing techniques
* PyTorch deep learning workflow
* GPU-based model training

---

## Author

Anshika Agarwal

---

