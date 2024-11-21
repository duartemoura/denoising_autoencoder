# Denoising Autoencoder

This project implements a denoising autoencoder using PyTorch to reconstruct clean images from noisy inputs. The model is trained on the MNIST dataset, which consists of handwritten digit images.
Overview

A denoising autoencoder is a type of neural network designed to remove noise from data. It learns to map noisy inputs to their original, noise-free versions, effectively learning a robust representation of the data.
Dataset

A model is trained on the MNIST and FMNIST dataset, which includes 60,000 training images and 10,000 test images of handwritten digits (0-9). Each image is 28x28 pixels in grayscale.

## Model Architecture

The autoencoder consists of two main parts:

    Encoder: Compresses the input image into a lower-dimensional latent representation.

    Decoder: Reconstructs the original image from the latent representation.

The architecture includes convolutional layers to capture spatial features effectively.

## Training

The model is trained to minimize the mean squared error between the original and reconstructed images. During training, random noise is added to the input images, and the autoencoder learns to reconstruct the original, noise-free images.

## Results

After training, the autoencoder successfully removes noise from the input images, producing clean reconstructions that closely resemble the original images.
