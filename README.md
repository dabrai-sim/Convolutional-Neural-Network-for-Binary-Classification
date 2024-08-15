# Convolutional Neural Network for Binary Classification (Cats vs Dogs)

## Project Overview
This project implements a Convolutional Neural Network (CNN) using TensorFlow and Keras to classify images of cats and dogs. The model is trained on an image dataset and predicts whether a given image is of a cat or a dog. The model is saved as an `.h5` file, and a script is provided to make single predictions.

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Model Architecture](#model-architecture)
- [Training and Evaluation](#training-and-evaluation)
- [Requirements](#requirements)

## Dataset
- The dataset used consists of two folders: `train` and `test`. Both folders contain two subfolders, `cats` and `dogs`, holding the respective images.
- The images are resized to 64x64 pixels before feeding them into the model.
- The dataset can be found using the following link: https://www.kaggle.com/c/dogs-vs-cats/data

## Model Architecture
1. Convolutional Layer: The model consists of two convolutional layers, each followed by a max-pooling layer.
2. Max Pooling: Pooling helps reduce the dimensionality of the feature maps.
3. Flattening: The 2D output from the convolutional layers is flattened into a 1D vector.
4. Dense Layers: A fully connected layer is used with 128 units and ReLU activation.
5. Output Layer: The final layer is a dense layer with a single unit and a linear activation for binary classification using hinge loss.

## Training and Evaluation
- The model is compiled with the `Adam` optimizer, `hinge` loss, and `accuracy` as the evaluation metric.
- The model is trained for 15 epochs with a batch size of 32, and both training and validation loss/accuracy are plotted.

## Requirements
To run this project, install the required dependencies using:


