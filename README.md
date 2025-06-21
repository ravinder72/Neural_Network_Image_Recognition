# Neural_Network_Image_Recognition
# 🧠 Neural_Network_Image_Recognition  
## Fashion MNIST Image Classifier using Deep Neural Network

This project implements a Deep Artificial Neural Network (ANN) trained on the [Fashion MNIST dataset](https://github.com/zalandoresearch/fashion-mnist) to classify grayscale clothing images into 10 predefined categories.

---

## 🧾 Project Overview

- **Input:** Grayscale images (28×28 pixels)
- **Output:** One of 10 fashion categories
- **Goal:** Accurately classify clothing images using a deep neural network

---

## 🧠 Model Architecture

The neural network is composed of:

- **Input Layer:**  
  - 784 features (flattened from 28×28 image)

- **Hidden Layer 1:**  
  - 128 neurons  
  - Activation: `ReLU`

- **Hidden Layer 2:**  
  - 128 neurons  
  - Activation: `ReLU`

- **Output Layer:**  
  - 10 neurons (for 10 classes)  
  - Activation: `Softmax`

---

## 🏷️ Fashion Labels

Each label corresponds to a specific clothing item:

```python
fashion_labels = {
    0: 'T-shirt/top',
    1: 'Trouser',
    2: 'Pullover',
    3: 'Dress',
    4: 'Coat',
    5: 'Sandal',
    6: 'Shirt',
    7: 'Sneaker',
    8: 'Bag',
    9: 'Ankle boot'
}