# Neural Network Classification with PyTorch

This notebook provides a comprehensive introduction to neural network classification using PyTorch, covering fundamental concepts from data preparation to model evaluation.

## Table of Contents

1.  **Making Classification Data and Getting It Ready**: Covers the generation of synthetic classification data (e.g., `make_circles`) and prepares it for model training, including converting data to tensors and creating train/test splits.

2.  **Building a Model**: Demonstrates how to construct a simple neural network model using `nn.Module` and `nn.Sequential` in PyTorch, setting up device-agnostic code, and defining loss functions (BCEWithLogitsLoss) and optimizers (SGD).

3.  **Training the Model**: Details the training loop process, including forward passes, loss calculation, backpropagation, and optimizer steps. It also explains how to convert model logits into prediction probabilities and labels.

4.  **Improving a Model**: Explores strategies for enhancing model performance, such as adding more layers and hidden units, increasing epochs, and considering different activation functions and learning rates. It includes a section on testing model capacity with linear regression data.

5.  **The Missing Piece: Non-Linearity**: Explains the importance of non-linear activation functions (like ReLU) in enabling neural networks to learn complex patterns, contrasting them with linear models. It also covers replicating activation functions manually.

6.  **Putting It All Together with a Multi-Class Classification Problem**: Extends the concepts to multi-class classification, demonstrating data creation with `make_blobs`, building a multi-class model, and using `nn.CrossEntropyLoss` and `softmax` for predictions.

7.  **Classification Metrics**: Introduces various evaluation metrics beyond accuracy, such as precision, recall, F1-score, confusion matrix, and classification report, using the `torchmetrics` library.

***[Open in Colab](https://colab.research.google.com/drive/1mvCQvxQIu3rHjg7G8LEthqc-gKUmBUIy?usp=sharing)***