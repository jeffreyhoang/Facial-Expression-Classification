# Facial Expression Classification

This project leverages a Convolutional Neural Network (CNN) built with PyTorch to classify facial expressions. With a test accuracy of **78%**, the model demonstrates effective performance in recognizing various expressions.

## 📚 Project Overview

Automatic facial expression classification has significant real-world applications, such as:
- Enhancing customer service systems
- Enabling personalized advertisements
- Improving entertainment experiences

The objective of this project is to develop a deep learning neural network model that accurately classifies facial expressions based on a given dataset.

## 🔍 Approach

### Data Transformations

To improve model generalization and performance, the following data transformations were applied:

- **Random Horizontal Flip**: Randomly flips images horizontally to introduce variability.
- **Random Rotation**: Rotates images within a range of -10 to +10 degrees, simulating slight head tilts.
- **Normalization**: Standardizes pixel values with a mean of 0.5 and a standard deviation of 0.5 to improve training stability.

### Model Architecture

The model architecture consists of a **four-layer CNN** for feature extraction, followed by fully connected layers for classification. The design details are as follows:

- **Convolutional Layers**: Each block includes a convolutional layer, batch normalization, ReLU activation, and max pooling, allowing the model to capture increasingly complex features at each layer.
- **Fully Connected Layers**: After flattening the output, the model uses three fully connected layers with ReLU activations, leading to the final classification layer.

This architecture enables the model to capture a hierarchy of features, essential for accurate facial expression recognition.

## 📈 Learning Curve

The learning curve below shows the training loss over epochs, illustrating the model's convergence:

<img width="471" alt="Screenshot 2024-11-04 at 11 26 40 PM" src="https://github.com/user-attachments/assets/3250cc4b-be8a-487b-9789-1c8efced866d">
