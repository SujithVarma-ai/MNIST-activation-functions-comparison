# Comparative Analysis of Sigmoid and ReLU Activation Functions for MNIST Image Classification

## 📌 Project Overview

This project presents a comparative analysis of **Sigmoid** and **ReLU (Rectified Linear Unit)** activation functions for handwritten digit classification using the **MNIST dataset**.

Two fully connected Artificial Neural Network (ANN) models with the same architecture were developed using **TensorFlow and Keras**. The primary difference between the two models is the activation function used in their hidden layers.

- **Model 1:** Sigmoid activation
- **Model 2:** ReLU activation

Both models were trained and evaluated using the same dataset, network architecture, optimizer, loss function, batch size, and number of epochs to provide a controlled comparison of the two activation functions.

---

## 🎯 Problem Statement

The performance of a neural network is influenced by several factors, including its architecture, training configuration, and activation functions.

Different activation functions can affect how a neural network learns patterns and how effectively it performs classification.

This project addresses the problem of comparing **Sigmoid and ReLU activation functions** under the same experimental conditions for handwritten digit classification.

The comparison is performed using:

- Test Accuracy
- Test Loss
- Confusion Matrix
- Precision
- Recall
- F1-Score
- Misclassified Images
- Training and Validation Performance

---

## 🎯 Objectives

The main objectives of this project are:

1. To preprocess and normalize the MNIST handwritten digit dataset.
2. To transform 28 × 28 pixel images into suitable input features for a fully connected neural network.
3. To design a neural network with the architecture **784–128–64–10**.
4. To implement two models using Sigmoid and ReLU activation functions.
5. To train both models under the same experimental configuration.
6. To evaluate both models using accuracy, loss, confusion matrices, and classification metrics.
7. To analyze the effect of activation-function selection on MNIST image classification performance.

---

## 📊 Dataset

The project uses the **MNIST handwritten digit dataset**.

MNIST contains grayscale images of handwritten digits from **0 to 9**, making it a **10-class image classification dataset**.

### Dataset Characteristics

| Property | Description |
|---|---|
| Dataset | MNIST |
| Total Images | 70,000 |
| Training Images | 60,000 |
| Test Images | 10,000 |
| Image Size | 28 × 28 pixels |
| Image Type | Grayscale |
| Number of Classes | 10 |
| Classes | Digits 0–9 |
| Input Features | 784 |

Each 28 × 28 image is flattened into a **784-dimensional vector** before being passed to the fully connected neural network.

### Dataset Split

The original 60,000 training images were further divided using a 10% validation split:

| Dataset | Images |
|---|---:|
| Training | 54,000 |
| Validation | 6,000 |
| Testing | 10,000 |

The 10,000 test images were kept separate and used only for final model evaluation.

---

## 🔄 Methodology

The overall workflow of the project is:

```text
MNIST Dataset
      ↓
Data Loading and Inspection
      ↓
Image Normalization
      ↓
Flatten 28 × 28 Images
      ↓
784 Input Features
      ↓
 ┌───────────────────────┐
 │                       │
 ↓                       ↓
Sigmoid Model          ReLU Model
784 → 128 → 64 → 10   784 → 128 → 64 → 10
 │                       │
 ↓                       ↓
Training                Training
 │                       │
 ↓                       ↓
Testing                 Testing
 │                       │
 └───────────┬───────────┘
             ↓
     Performance Evaluation
             ↓
 Accuracy | Loss | Confusion Matrix
 Precision | Recall | F1-Score
             ↓
       Model Comparison
             ↓
    Final Results and Insights
```

## Neural Network Architecture

```text
Input Layer
784 neurons
    ↓
Hidden Layer 1
128 neurons
    ↓
Hidden Layer 2
64 neurons
    ↓
Output Layer
10 neurons
```
