# Image Classification with TensorFlow

This project implements a deep learning model for image classification using TensorFlow and Keras. The model is trained on the **Fashion MNIST dataset**, which contains 70,000 grayscale images of 10 different types of clothing.

---

## 📌 Project Overview

This notebook demonstrates how to:

* Load and preprocess the Fashion MNIST dataset.
* Build a neural network using TensorFlow/Keras.
* Train the model on the training dataset.
* Evaluate its performance on unseen data.
* Make predictions and visualize results.

---

## 📂 Dataset

**Fashion MNIST** is a drop-in replacement for the original MNIST dataset but with images of clothing items instead of handwritten digits.

* **Classes**:

  * `T-shirt/top`, `Trouser`, `Pullover`, `Dress`, `Coat`,
  * `Sandal`, `Shirt`, `Sneaker`, `Bag`, `Ankle boot`
* **Image Size**: 28x28 grayscale
* **Training samples**: 60,000
* **Test samples**: 10,000

---


## 🚀 Model Architecture


* **Input Layer**: Flattens 28x28 images into 784-dimension vectors
* **Hidden Layer**: 128 neurons, ReLU activation
* **Output Layer**: 10 neurons (one for each clothing class)



---

## 📊 Prediction Output

The model outputs a probability distribution over the 10 classes. A helper function visualizes:

* The predicted label vs actual label.
* A bar graph showing model confidence.

```python
np.argmax(predictions[0])  # Predicted label
test_labels[0]             # Actual label
```

✅ **Correct predictions are shown in blue**, ❌ **incorrect ones in red**.

---

## 💡 Key Learnings

* Understanding the workflow of TensorFlow/Keras for image classification.
* Importance of data preprocessing (normalization).
* Model evaluation using validation accuracy and prediction confidence.


