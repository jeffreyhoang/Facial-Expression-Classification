# Facial Expression Classification

This project focuses on classifying facial expressions using a Convolutional Neural Network (CNN) built with PyTorch. The model achieved an accuracy of 78% on the test dataset, demonstrating effective performance in recognizing facial expressions across different classes.
Approach

Data Transformations
To enhance model generalization, the following transformations were applied to the training data:
Random Horizontal Flip: Introduces variety by flipping images horizontally.
Random Rotation: Rotates images within a range of -10 to +10 degrees.
Normalization: Standardizes pixel values with a mean of 0.5 and a standard deviation of 0.5.
These transformations help the model learn robust features by introducing slight variations in the input images.
Model Architecture
The model consists of a four-layer CNN for feature extraction, followed by fully connected layers for classification. Key elements include:
Convolutional Blocks: Each block contains a convolutional layer, batch normalization, ReLU activation, and max pooling.
Fully Connected Layers: After flattening, the model has three fully connected layers with ReLU activations, leading to the final classification output.
This architecture enables the model to capture a hierarchy of features, essential for accurate facial expression recognition.
Learning Curve

The learning curve below shows the training loss over epochs, illustrating the model's convergence:
python