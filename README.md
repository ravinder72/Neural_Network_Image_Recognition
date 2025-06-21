# Neural_Network_Image_Recognition
# 🧠 Fashion MNIST Image Classifier using Deep Neural Network

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

---

## ⚙️ Training Configuration
- **Loss Function:** Loss_CategoricalCrossentropy()

- **Optimizer:** Optimizer_Adam(decay=1e-3)

- **Accuracy Metric:** Accuracy_Categorical()

- **Activations:**

    -Hidden Layers: `ReLU`

    -Output Layer: `Softmax`

---

## 🧪 Data Preprocessing
-**Before training, the following steps are performed:**

  -Normalize pixel values (typically scaled between 0 and 1)

  -Flatten 28×28 images into 784-element vectors

  -One-hot encode the labels for categorical classification

---

## 💾 Model Persistence
-**After training:**

  -The model is saved to disk

  -You can load and use the model directly for inference without retraining

---

## 🔄 Example Usage
  -python
  -Copy
  -Edit
# Load the trained model
  -model.load('your_model_file_path')

---

# Predict using test data
-predictions = model.predict(X_test)

---

📦 Dataset Details
-**The Fashion MNIST dataset is a drop-in replacement for the original MNIST digits dataset and includes:**

  -60,000 training images

  -10,000 testing images

  -10 classes of fashion items

  -Each image is grayscale, 28×28 pixels

---

## ✅ Dependencies
-**Make sure the following components or libraries are available (or implemented if custom):**

  -Layers (Dense, Activation)

  -Optimizer (Adam)

  -Loss Function (Categorical Crossentropy)

  -Accuracy Metrics

  -Dataset Loader (Fashion MNIST)

  -Model Save/Load functionality

---

## 📌 Summary
This project showcases the power of deep learning applied to image classification. The model architecture, training strategy, and data preprocessing work together to achieve accurate predictions on a diverse set of fashion items. Once trained, the model is efficient, fast, and ready for deployment.

---

## 📄 License
This project is for educational purposes. Feel free to use or modify it as needed!