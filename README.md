# Facial-Emotions-Detection-

## Table of Contents
Introduction  
Dataset (FER2013)  
Model (CNN)  
Requirements  
Usage

## Introduction
The project focuses on creating a real-time facial emotion detection system using a Convolutional Neural Network (CNN) model. The CNN was trained on the FER2013 dataset, which contains facial images labeled with different emotions such as happy, sad, angry, etc. The goal is to utilize deep learning and computer vision techniques to detect and recognize emotions from faces in real-time.

## Dataset (FER2013)
The FER2013 dataset is a widely used dataset for facial emotion recognition. It contains over 35,000 grayscale images of faces labeled with one of seven emotions: angry, disgust, fear, happy, sad, surprise, and neutral. The dataset is split into training, validation, and test sets.

## Advanced Preprocessing 
Data Augmentation:
Augmentation methods like rotation, horizontal and vertical flipping, random cropping, brightness adjustments, and zooming were used to create diverse variations of facial images.
Increases data variability, making the model more robust and less prone to overfitting.

Image Reshaping and Normalization:
All facial images were resized to a fixed dimension for uniformity in input size.
Pixel values were normalized to [0, 1] or [-1, 1] to bring them into a common scale, stabilizing the training process.

Label Integer Mapping:
Emotion labels were mapped to integer values (e.g., "happy" to 0, "sad" to 1) instead of one-hot encoding.
Simplifies label representation and reduces memory requirements during training.


## Model (CNN)
The Convolutional Neural Network (CNN) is a deep learning architecture well-suited for image recognition tasks. The CNN model was designed and created specifically for facial emotion recognition. It consists of multiple convolutional and pooling layers to extract relevant features from the facial images. The output layer uses softmax activation to predict the probabilities of different emotions for a given input face.

# Requirements
To run the facial emotion detection system, make sure you have the following dependencies installed:

Python (>=3.6)  
NumPy (>=1.18.5)  
OpenCV (cv2)  
TensorFlow (>=2.0)  
