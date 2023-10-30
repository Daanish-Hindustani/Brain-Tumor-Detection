# Convolutional Neural Network for Brain Tumor Classification
<img width="948" alt="Screenshot 2023-10-29 at 10 28 19 PM" src="https://github.com/Daanish-Hindustani/Brain-Tumor-Detection/assets/134811343/e25f182f-63fd-4695-a621-3af174238988">





## Overview
This repository contains a Convolutional Neural Network (CNN) for brain tumor classification using an enhanced dataset. The dataset includes four types of tumors: Glioma Tumor, Meningioma Tumor, Normal, and Pituitary Tumor. The dataset distribution is as follows:

Glioma Tumor: 901 samples
Meningioma Tumor: 913 samples
Normal: 438 samples
Pituitary Tumor: 844 samples
The data has undergone significant enhancements to improve data quality and consistency. The neural network trained on this dataset has achieved a training accuracy of 99% and a testing accuracy of 85%. The training and testing split used was 80% for training and 20% for testing.

## Introduction
This enhanced dataset aims to provide a reliable and standardized resource for advanced medical research in brain tumor classification. It builds upon the work of the original dataset while introducing several key enhancements to improve data quality and consistency.

## Data Source
The initial data was sourced from the brain tumor classification MRI dataset, which is accessible at this link and was generously shared by Sartaj. We would like to express our gratitude for making this valuable dataset available.

## Enhancements Made
Removal of Redundant Data
To ensure the consistency and reliability of the dataset, redundant data has been removed. This includes data augmentations like Salt and Pepper noise and geometric transformations. The elimination of these augmentations helps ensure that the dataset is free from unnecessary variations.

## Image Normalization
All images in the dataset have undergone grayscale histogram-based normalization. This process enhances image quality and comparability by standardizing the intensity levels of the images. Normalization is a crucial step in preprocessing medical images for machine learning applications.

## Resizing with Aspect Ratio Preservation
To create a uniform dataset for training and testing, all images have been resized to a consistent 256 x 256-pixel size. Importantly, the original aspect ratio of the images has been preserved during resizing. This ensures that important details in the images are retained, and the model can learn from consistent data.

## Neural Network Architecture

The neural network architecture implemented for brain tumor classification is designed to efficiently process and classify medical images. Here, we will discuss the architecture without delving into the specific code implementation.

### Convolutional Layer

The neural network begins with a convolutional layer. This layer is responsible for learning relevant image features. It applies 16 convolutional filters to the input images, with each filter learning different patterns or features. The filters have a size of (3, 3) and use the Rectified Linear Unit (ReLU) activation function, introducing non-linearity.

### Max-Pooling Layer

After the initial convolutional layer, a max-pooling layer is introduced. Max-pooling is a down-sampling operation that reduces the spatial dimensions of the feature maps. It helps to retain essential information while decreasing computational complexity.

### Fully Connected (Dense) Layers

The neural network includes two fully connected dense layers. These dense layers follow the convolutional and max-pooling layers and are crucial for making high-level decisions based on the features learned in the earlier layers.

- The first dense layer, with 256 units and ReLU activation, is responsible for extracting complex and high-level features from the data.
- The second dense layer serves as the output layer, where the network provides classification results. It has four units, each representing one of the four classes: Glioma Tumor, Meningioma Tumor, Normal, and Pituitary Tumor. The softmax activation function converts the network's raw output into class probabilities, making it suitable for multi-class classification.

### Dropout Layer

To prevent overfitting and improve the model's generalization, a dropout layer is included. The dropout layer randomly deactivates a fraction of input units during training, ensuring that the model does not rely too heavily on any specific feature.

This architecture combines convolutional layers to learn relevant image features and fully connected layers for making classification decisions. The combination of these layers, along with the use of activation functions and dropout, enables the model to efficiently classify brain tumor images into the respective categories. The training and testing accuracy achieved by this architecture reflect its effectiveness in the classification task. 

## Neural Network Performance
The Convolutional Neural Network (CNN) trained on this enhanced dataset has achieved the following performance:

Training Accuracy: 99%
Testing Accuracy: 85%
This level of accuracy showcases the effectiveness of the dataset enhancements and the potential of the neural network for brain tumor classification.

## Training Accuracy Over 5 EPOCHs
<img width="575" alt="Screenshot 2023-10-29 at 10 23 07 PM" src="https://github.com/Daanish-Hindustani/Brain-Tumor-Detection/assets/134811343/50a4282c-619c-408e-9639-18d76d768886">



## Testing Accuracy 
<img width="588" alt="Screenshot 2023-10-29 at 10 23 57 PM" src="https://github.com/Daanish-Hindustani/Brain-Tumor-Detection/assets/134811343/5d05afbd-d606-41f0-a618-59310d1eb88d">



## Input Of Unkownn Tumor 
![unknown_tumor](https://github.com/Daanish-Hindustani/Brain-Tumor-Detection/assets/134811343/64c3bd02-2629-47d5-b4f3-a13fcdafe907)

<img width="871" alt="Screenshot 2023-10-30 at 9 27 48 AM" src="https://github.com/Daanish-Hindustani/Brain-Tumor-Detection/assets/134811343/b7c920d6-0015-4466-a66e-e15a462a4756">

<img width="843" alt="Screenshot 2023-10-30 at 9 28 13 AM" src="https://github.com/Daanish-Hindustani/Brain-Tumor-Detection/assets/134811343/507325d4-1319-4138-9600-635d81172a5d">





