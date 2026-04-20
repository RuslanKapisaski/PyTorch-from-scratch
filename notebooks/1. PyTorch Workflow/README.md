# PyTorch Workflow Notebook

This notebook demonstrates a basic end-to-end PyTorch workflow for a linear regression model. It covers the essential steps from data preparation to saving and loading the trained model.

## Table of Contents

1.  Data Preparation and Loading
2.  Splitting Data into Training and Test Sets
3.  Building a Model
4.  Training the Model
5.  Saving and Loading Models
6.  Putting It All Together (Refactored Workflow)

## 1. Data Preparation and Loading

-   **Objective**: Create synthetic linear data (`y = weight * X + bias`) for demonstration.
-   **Key Steps**: 
    -   Define known parameters `weight` and `bias`.
    -   Generate `X` values using `torch.arange`.
    -   Calculate `y` based on `X`, `weight`, and `bias`.

## 2. Splitting Data into Training and Test Sets

-   **Objective**: Divide the generated data into training and testing subsets.
-   **Key Concepts**: Introduction to training, validation, and test sets, crucial for evaluating model performance.
-   **Visualization**: A helper function `plot_predictions` is defined to visualize the data splits.

## 3. Building a Model

-   **Objective**: Implement a simple linear regression model using PyTorch's `nn.Module`.
-   **Key PyTorch Components**: 
    -   `torch.nn`: Building blocks for neural networks.
    -   `torch.nn.Parameter`: Learnable parameters (weights and biases).
    -   `torch.nn.Module`: Base class for all neural network modules.
    -   `forward()`: Defines the computation performed by the model.
-   **Initial State**: The model starts with random `weights` and `bias` values.

## 4. Training the Model

-   **Objective**: Adjust the model's parameters to minimize the difference between predictions and actual values.
-   **Key Components**: 
    -   **Loss Function (`nn.L1Loss`)**: Measures how far off the model's predictions are.
    -   **Optimizer (`torch.optim.SGD`)**: Adjusts model parameters based on the loss (using gradient descent).
-   **Training Loop**: Iterates through epochs, performing:
    -   Forward pass
    -   Loss calculation
    -   Backpropagation
    -   Optimizer step
-   **Evaluation**: The model is set to `eval()` mode for testing, using `torch.inference_mode()`.

## 5. Saving and Loading Models

-   **Objective**: Demonstrate how to persist and retrieve trained models.
-   **Methods**: 
    -   `torch.save()`: Saves the model's `state_dict()` (recommended).
    -   `torch.load()`: Loads a saved state dictionary.
    -   `model.load_state_dict()`: Applies the loaded state to a new model instance.

## 6. Putting It All Together (Refactored Workflow)

-   **Objective**: Re-implement the entire workflow in a more organized and device-agnostic manner.
-   **Improvements**: 
    -   Device-agnostic code (`cuda` or `cpu`).
    -   Uses `nn.Linear` layer for cleaner model definition (`LinearRegressionModelv2`).
    -   Consolidates the training and testing loops.
-   **Verification**: Compares predictions of the original and loaded models to ensure correctness.

This notebook serves as a foundational example for understanding the core concepts of building and training simple neural networks in PyTorch.
---
***[Open in Colab](https://colab.research.google.com/drive/1XohPrgSqy-KVEfhIaYRsi0ZNas7QD2IX?usp=sharing)***