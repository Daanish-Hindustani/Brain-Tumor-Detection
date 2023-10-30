# Convolutional Neural Network for Brain Tumor Classification

This repository contains a Convolutional Neural Network (CNN) for brain tumor classification using an enhanced dataset. The dataset is built upon the "Uncovering Knowledge: A Clean Brain Tumor Dataset for Advanced Medical Research" and has undergone significant improvements while acknowledging the original authors' contributions. The neural network has achieved a training accuracy of 99% and a testing accuracy of 85%.

## Introduction

This enhanced dataset aims to provide a reliable and standardized resource for advanced medical research in brain tumor classification. It builds upon the work of the original dataset while introducing several key enhancements to improve data quality and consistency.

## Data Source

The initial data was sourced from the brain tumor classification MRI dataset, which is accessible at [this link](original_data_source_link) and was generously shared by Sartaj. We would like to express our gratitude for making this valuable dataset available.

## Enhancements Made

### Removal of Redundant Data

To ensure the consistency and reliability of the dataset, redundant data has been removed. This includes data augmentations like Salt and Pepper noise and geometric transformations. The elimination of these augmentations helps ensure that the dataset is free from unnecessary variations.

### Image Normalization

All images in the dataset have undergone grayscale histogram-based normalization. This process enhances image quality and comparability by standardizing the intensity levels of the images. Normalization is a crucial step in preprocessing medical images for machine learning applications.

### Resizing with Aspect Ratio Preservation

To create a uniform dataset for training and testing, all images have been resized to a consistent 256 x 256-pixel size. Importantly, the original aspect ratio of the images has been preserved during resizing. This ensures that important details in the images are retained, and the model can learn from consistent data.

## Neural Network Performance

The Convolutional Neural Network (CNN) trained on this enhanced dataset has achieved the following performance:

- Training Accuracy: 99%
- Testing Accuracy: 85%

This level of accuracy showcases the effectiveness of the dataset enhancements and the potential of the neural network for brain tumor classification.

## Usage

To use this dataset and train your own neural network for brain tumor classification, follow the instructions in the provided code. You can find the neural network architecture, training process, and evaluation metrics in the codebase.

