# 👕 FashionMNIST Classification: From Linear Models to CNNs

## 📌 Overview
This project explores computer vision and deep learning by building progressive models to classify clothing items using the **FashionMNIST** dataset. Rather than jumping straight to complex architectures, this project documents the journey from a simple baseline model to a fully convolutional neural network, tracking performance and training time along the way.

## 🛠️ Tech Stack & Tools
- **Framework:** PyTorch (`torch`, `torch.nn`, `torchvision`)
- **Data Handling:** `torch.utils.data.DataLoader` (Python Iterators)
- **Performance Tracking:** `timeit` (Benchmarking CPU vs. GPU training time)
- **Optimization:** Stochastic Gradient Descent (SGD)
- **Loss Function:** Cross Entropy Loss

---

## 🏗️ Model Architectures Explored

This project implements three distinct models to demonstrate the impact of different architectural choices:

### 1. Model 0: The Baseline (Linear)
A simple Artificial Neural Network (ANN) using only `nn.Linear` layers. 
- **Purpose:** To establish a baseline accuracy and training time.

### 2. Model 1: Introducing Non-Linearity
An ANN identical to Model 0, but with `ReLU` (Rectified Linear Unit) activation functions injected between the linear layers.
- **Purpose:** To observe how non-linear activation helps the network learn complex patterns in the image data.

### 3. Model 2: TinyVGG (CNN)
A Convolutional Neural Network replicating the **TinyVGG** architecture. 
- **Purpose:** To utilize convolutional layers to extract spatial features (edges, shapes) from the clothing images, representing a standard modern approach to computer vision.

---

## 📊 Training & Evaluation

To ensure rigorous evaluation, the dataset was formally split into **Train** and **Test** sets. 

A custom helper function was written to calculate **Accuracy**, allowing for a direct comparison across all three models. Additionally, the `timeit.default_timer()` was used to benchmark hardware performance, specifically comparing **CPU vs. GPU** execution times for deep learning workloads.

### Results Summary
*(Note: Replace the bracketed text with your actual results before saving!)*

| Model | Architecture | Device | Training Time | Test Accuracy |
| :--- | :--- | :--- | :--- | :--- |
| **Model 0** | Linear Baseline | [CPU/GPU] | [e.g., 25 seconds] | [e.g., 78%] |
| **Model 1** | Linear + ReLU | [CPU/GPU] | [e.g., 28 seconds] | [e.g., 81%] |
| **Model 2** | TinyVGG (CNN) | GPU | [e.g., 15 seconds] | [e.g., 90%+] |

---

## 🚀 How to Run

1. Clone this repository:
   ```bash
   git clone 
