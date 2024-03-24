# Handwritten Digit Recognition with Convolutional Neural Networks
This project implements a Convolutional Neural Network (CNN) using TensorFlow in Python to recognize handwritten digits from the MNIST dataset.

# Overview
This project is completed as part of the certificate program on Convolutional Neural Networks with TensorFlow offered by 365 Data Science. The model architecture and training process aim to achieve high accuracy in digit recognition tasks.

# Author
Mohamed Manessouri
Smart System Engineering Student
ENSIAS, Morocco

# Dataset
The MNIST dataset consists of 60,000 training images and 10,000 testing images of handwritten digits (0 to 9) with corresponding labels. Each image is grayscale and has a resolution of 28x28 pixels.

# Preprocessing
The dataset is loaded using TensorFlow Datasets (tfds).
Images are scaled to the range [0, 1].
Training and validation datasets are prepared.
Data is batched and shuffled for training.



# Model Architecture

The CNN model comprises the following layers:
Convolutional layer (50 filters, kernel size 5x5, ReLU activation)
MaxPooling layer (2x2)
Convolutional layer (50 filters, kernel size 3x3, ReLU activation)
MaxPooling layer (2x2)
Flatten layer
Dense layer (10 units, output layer)

# Training
Adam optimizer is used with Sparse Categorical Crossentropy loss function.
Training is performed over 20 epochs with early stopping.
TensorBoard is utilized for visualization and monitoring training progress.
Confusion matrix is logged to evaluate model performance on validation data.


# Testing
Model performance is evaluated on the test dataset.
Test accuracy and loss are reported.
Random test images are selected for visualization.
Predictions are made and probability distributions are visualized.

