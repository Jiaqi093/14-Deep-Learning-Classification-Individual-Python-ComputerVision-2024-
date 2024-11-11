## Background
In this task, we train a Convolutional Neural Network (CNN) on the Fashion-MNIST dataset to classify images into ten categories of clothing. This dataset contains grayscale images of 28x28 pixels across 70,000 samples, with labels spanning ten clothing types. The objective is to build a CNN model capable of accurately classifying these images while exploring techniques to enhance performance and efficiency.

## Process Overview
1. Data Preparation:

* Downloaded the Fashion-MNIST dataset, which includes 60,000 training images (with an additional split for validation) and 10,000 test images.
* Normalized images to the range (-1, 1) and applied data augmentation techniques such as random horizontal flipping and padding with cropping to improve model generalization.

2. Model Architecture:
The CNN architecture includes:

* Layer 1: A 5x5 convolutional layer with 32 filters, ReLU activation, followed by a 2x2 max pooling layer.
* Layer 2: A 3x3 convolutional layer with 64 filters, ReLU activation, followed by another 2x2 max pooling layer.
* Fully Connected Layers: A fully connected layer with 1024 output units, ReLU activation, and an output layer with ten units.

3. Training Configuration:
* Loss Function: Cross-entropy loss to measure classification accuracy.
* Optimizer: Adam optimizer with a learning rate of 1 × 10^(−3) to improve convergence.
* Tracking Performance: Monitored training and validation loss and accuracy over epochs to evaluate model learning.
  
4. Results:
* Plotted training and validation accuracy/loss trends across epochs.
* Tested various improvements (e.g., adding batch normalization, dropout) to enhance accuracy and prevent overfitting.
  
5. Comparative Analysis:
* Compared the CNN model’s performance with other models like ResNet18, discussing the impact of ResNet’s deeper layers and residual connections on accuracy and gradient flow.
