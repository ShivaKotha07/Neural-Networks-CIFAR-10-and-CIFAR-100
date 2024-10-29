# CIFAR-10 and CIFAR-100 Image Classification using Convolutional Neural Networks

# Importing Libraries: 
The code starts by importing the necessary libraries and modules from the Keras deep learning framework, as well as NumPy and Matplotlib for data processing and visualization.
Loading and Preprocessing CIFAR-10 Dataset: The code loads the CIFAR-10 dataset, which contains 60,000 32x32 color images in 10 different classes (airplane, automobile, bird, cat, deer, dog, frog, horse, ship, and truck). It then performs the following preprocessing steps:

Converts the pixel values to float32 data type
Normalizes the pixel values to the range [0, 1]
Converts the labels to one-hot encoded format


# Creating the CNN Model: 
The code then defines a Convolutional Neural Network (CNN) model using the Keras Sequential API. The model consists of the following layers:
2 sets of Convolutional, Batch Normalization, and MaxPooling layers with Dropout
2 more sets of Convolutional, Batch Normalization, and AveragePooling layers with Dropout
A Flatten layer to convert the 2D feature maps to a 1D feature vector
2 Dense layers with Batch Normalization and Dropout for classification


# Training the Model: 
The code compiles the model with the Adam optimizer and categorical cross-entropy loss, and then trains the model on the CIFAR-10 dataset for 100 epochs, using a batch size of 64. It also includes the validation dataset to monitor the model's performance during training.
Evaluating the Model: After training, the code prints the average training and validation accuracy, as well as the average training and validation loss.

# Visualizing the Results: 
The code generates two plots: one for the loss curves (training and validation) and one for the accuracy curves (training and validation) during the training process.

# Repeating the Process for CIFAR-100: 
The code then repeats a similar process for the CIFAR-100 dataset, which has 100 classes instead of 10. The model architecture is slightly modified, with some changes in the number of filters and pooling layers.

This code provides a comprehensive example of how to build and train a CNN model using the Keras library for image classification tasks, specifically on the CIFAR-10 and CIFAR-100 datasets. The key aspects of the code include data loading and preprocessing, model definition, training, evaluation, and visualization of the results. Understanding this code will help you develop a solid foundation in deep learning for image classification problems.
