# PyTorch Custom Datasets Notebook

This notebook explores different ways to load and prepare image data for deep learning models in PyTorch, focusing on both standard `ImageFolder` usage and creating custom `Dataset` implementations. It also covers data augmentation and demonstrates training a simple CNN (TinyVGG) with and without augmentation.

## Table of Contents

- Importing PyTorch and setting up device-agnostic code
- Getting and exploring data (pizza, steak, sushi dataset)
- Data Transformation with `torchvision.transforms`
- Loading Data using `ImageFolder` and `DataLoader`
- Creating a Custom `Dataset` and `DataLoader`
- Data Augmentation Techniques (e.g., `TrivialAugmentWide`)
- Model 0: TinyVGG without data augmentation (training and evaluation)
- Model 1: TinyVGG with data augmentation (training and evaluation)
- Comparison of model results
- Making predictions on custom images

## Key Learnings

- How to download and prepare image datasets.
- Visualizing raw and transformed images.
- Using `torchvision.datasets.ImageFolder` for efficient data loading.
- Implementing a custom `torch.utils.data.Dataset` for more control over data handling.
- Applying data augmentation using `torchvision.transforms` to improve model robustness.
- Building and training a basic Convolutional Neural Network (TinyVGG).
- Evaluating model performance and plotting loss curves.
- Making predictions on new, unseen images.

---
***[Open in Colab](https://colab.research.google.com/drive/1wVtswPXt1rLGnQ7iJ-sSMy665i-yrdt1?usp=sharing)***