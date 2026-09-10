# 👕 Enhanced CVAE for Fashion-MNIST

Conditional Variational Autoencoder with advanced latent-space optimization techniques.
## Overview

This project implements a Conditional Variational Autoencoder (CVAE) using PyTorch for image generation on the Fashion-MNIST dataset.

The objective is to generate realistic clothing images conditioned on class labels while improving latent-space representations and sample quality through several advanced techniques.

## Dataset

Fashion-MNIST is a dataset of 70,000 grayscale images across 10 clothing categories:

- T-shirt/Top
- Trouser
- Pullover
- Dress
- Coat
- Sandal
- Shirt
- Sneaker
- Bag
- Ankle Boot

## Implemented Improvements

### Conditional Batch Normalization (CBN)

Condition class information directly into normalization layers to improve class-specific generation.

### KL Annealing

Gradually increase the KL divergence weight during training to avoid posterior collapse and stabilize optimization.

### Normalizing Flows

Increase the flexibility of the latent distribution and improve approximation of complex posterior distributions.

### Conditioning Mechanism

Class labels are integrated into both encoder and decoder networks to guide image generation.

## Experiments

Several experiments were conducted to evaluate the impact of:

- Latent dimension size
- Learning rate
- KL annealing schedules
- Batch size
- Conditional Batch Normalization
- Normalizing Flow layers
