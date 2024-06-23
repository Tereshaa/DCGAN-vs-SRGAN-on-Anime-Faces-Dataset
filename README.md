# DCGAN vs SRGAN on Anime Faces Dataset

This repository explores and compares the performance of two popular Generative Adversarial Networks (GANs) — DCGAN (Deep Convolutional Generative Adversarial Network) and SRGAN (Super-Resolution Generative Adversarial Network) — on the Anime Faces dataset. 

## Overview

### DCGAN (Deep Convolutional GAN)
DCGAN is a foundational GAN architecture designed for generating new images from random noise. It uses convolutional networks in both the generator and discriminator to learn the distribution of images in the training data and generate new, realistic-looking images.

### SRGAN (Super-Resolution GAN)
SRGAN is specialized in generating high-resolution images from low-resolution inputs. It incorporates perceptual loss functions alongside adversarial loss to produce images with enhanced details and realism.

## Dataset
The Anime Faces dataset consists of images of anime-style faces, typically used for character generation and digital art. This dataset is available on [Kaggle](https://www.kaggle.com/datasets/soumikrakshit/anime-faces)
## Implementation Details
- **DCGAN Implementation**:
  - Utilizes a generator that starts with a dense layer followed by transposed convolutional layers to upsample noise into anime-style images.
  - The discriminator consists of convolutional layers with batch normalization and LeakyReLU activations.

- **SRGAN Implementation**:
  - Features a generator that includes convolutional layers and upscaling through transposed convolutions to enhance the resolution of low-resolution anime faces.
  - The discriminator is designed to distinguish between real high-resolution anime faces and generated high-resolution outputs.

## Training
- Both models are trained over 50 epochs on the Anime Faces dataset.
- Training metrics such as discriminator loss (d_loss) and generator loss (g_loss) are monitored to evaluate and compare their performance.

## Results
- After training, the models' performance is assessed based on their ability to generate realistic anime faces and enhance image resolution.
- Differences in d_loss and g_loss provide insights into each model's strengths and limitations in generating and enhancing anime faces.
