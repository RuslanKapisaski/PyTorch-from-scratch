# PyTorch Computer Vision with FashionMNIST
This notebook demonstrates fundamental concepts in computer vision using PyTorch, focusing on image classification with the FashionMNIST dataset.

## Table of Contents
1. Computer Vision Libraries
Introduces key PyTorch libraries for computer vision, such as torchvision, torch.nn, and matplotlib.

2. Getting a Dataset
Loads and explores the FashionMNIST dataset, including checking image shapes, labels, and visualizing samples.

3. Prepare DataLoader
Transforms the dataset into iterable DataLoader objects for efficient batch processing during model training and evaluation.

4. Model 0: Build a Baseline Model
Develops a simple baseline neural network (FashionMNISTModelV0) using a Flatten layer and Linear layers to classify images. It also covers setting up loss, optimizer, and evaluation metrics, along with a basic training loop.

5. Setup Device Agnostic Code
Configures the environment to utilize a GPU (if available) for faster computations.

6. Build a Better Model with Non-linearity
Introduces FashionMNISTModelV1, an improved model incorporating a ReLU activation function to add non-linearity, enhancing its learning capability.

7. Model 2: Building a Convolutional Neural Network (CNN)
Constructs a more advanced FashionMNISTModelV2 (a simple CNN) to leverage the power of convolutional layers for image feature extraction, typically leading to higher performance in vision tasks.

8. Comparing Model Results and Training Time
Compares the performance (accuracy, loss) and training times of all three models (V0, V1, V2) to highlight the benefits of more complex architectures.

9. Make and Evaluate Random Predictions with Best Model
Demonstrates how to make predictions on new, unseen images using the best-performing model and visually inspects the results against true labels.

10. Making a Confusion Matrix for Further Prediction Evaluation
Generates and plots a confusion matrix to provide a detailed breakdown of model performance, showing correct and incorrect classifications for each class.

11. Save and Load the Best Performing Model
Illustrates the process of saving the trained model's state dictionary and loading it back, ensuring reproducibility and easy deployment.

***[Open in Colab](https://colab.research.google.com/drive/1DX4OKRz9JnDiugVEO_P9FMT3SF18a5kP?usp=sharing)***