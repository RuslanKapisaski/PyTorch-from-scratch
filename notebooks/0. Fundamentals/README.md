# Introduction to PyTorch Tensors

This notebook provides comprehensive introduction to PyTorch tensors, covering fundamental operations and concepts essential for deep learning in Google Colab.

## Table of Contents

1. Creating Tensors
    *   Random Tensors
    *   Tensors of Zeros and Ones
    *   Creating a Range of Tensors and Tensors-like
2.  Tensor Datatypes
    *   Getting Tensor Information
    *   Tensor Operations
    *   Tensor Aggregation
    *   Reshaping, Stacking, Squeezing and Unsqueezing Tensors
    *   Indexing (Selecting Data from Tensors)
3.  PyTorch Tensors & NumPy
4.  Reproducibility (Random Seeds)
5.  Running Tensors and PyTorch Objects on GPUs

## Key Concepts Covered:

*   **Tensor Creation**: Demonstrates how to create scalars, vectors, matrices, and higher-dimensional tensors.
*   **Random Tensors**: Explains the importance and creation of random tensors for neural network initialization.
*   **Special Tensors**: Shows how to create tensors filled with zeros or ones, and tensors within a specified range (`torch.arange`).
*   **Tensor Properties**: Covers how to inspect `dtype`, `shape`, `ndim` (number of dimensions), and `device` of tensors.
*   **Basic Operations**: Illustrates element-wise addition, subtraction, multiplication, and division.
*   **Matrix Multiplication**: Explores matrix multiplication, including handling shape errors with `.T` (transpose) and `torch.mm`.
*   **Aggregation**: Shows how to find min, max, mean, sum, `argmin`, and `argmax` of tensors.
*   **Reshaping & Views**: Explains `reshape()`, `view()`, `stack()`, `squeeze()`, `unsqueeze()`, and `permute()` for manipulating tensor dimensions.
*   **Indexing**: Demonstrates how to access specific elements or slices of tensors using various indexing techniques.
*   **Interoperability with NumPy**: Covers conversion between PyTorch tensors and NumPy arrays, and important considerations regarding shared memory and data types.
*   **Reproducibility**: Introduces `torch.manual_seed()` for ensuring reproducible random tensor generation.
*   **GPU Usage**: Explains how to set up device-agnostic code, check for GPU availability, and move tensors between CPU and GPU for faster computations.

---
***[Open in Colab](https://colab.research.google.com/drive/1FX9tKfnSz3DlId28krvUp4VMfR8Clhc8?usp=sharing)***