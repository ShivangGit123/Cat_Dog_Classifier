# Cat_Dog_Classifier

This project implements a Convolutional Neural Network (CNN) using TensorFlow/Keras to classify images as either dogs (`0`) or cats (`1`).

## Project Overview

The objective is to build a deep learning model that can automatically identify whether an image contains a dog or a cat. The model is trained on labeled images and uses CNN layers to extract relevant features.

## Dataset

- Input: RGB images resized to 256x256 pixels
- Labels:
  - 0 = Dog
  - 1 = Cat

(Note: Dataset is assumed to be locally available or uploaded via Google Colab.)

## Model Architecture

- Convolutional + MaxPooling layers:
  - Conv2D with 32 filters → MaxPooling
  - Conv2D with 64 filters → MaxPooling
  - Conv2D with 128 filters → MaxPooling
- Flatten layer
- Dense layers:
  - Dense(128) → Dense(64) → Dense(1)
- Activation functions:
  - ReLU for hidden layers
  - Sigmoid for binary output

## Technologies Used

- Python
- TensorFlow / Keras
- NumPy
- OpenCV (cv2) for image handling
- Google Colab (for training and testing)

## Results

- The model outputs a probability between 0 and 1
  - Values closer to 0 are classified as "Dog"
  - Values closer to 1 are classified as "Cat"
