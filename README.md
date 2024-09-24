# 🖋️ Handwritten Digit Classification with Keras

This project implements a neural network model for classifying handwritten digits using the famous MNIST dataset. The model is built using the Keras library and consists of 728 input nodes, a hidden layer of 128 nodes, and 10 output nodes representing the digit classes (0–9).

## 🧠 Model Architecture

### Input Layer
- The input layer consists of **728 nodes**, which corresponds to the flattened 28x28 pixel images from the MNIST dataset.

### Hidden Layer
- A single **Dense layer** with **128 neurons** is used to learn the complex features of the digits.

### Output Layer
- The output layer has **10 neurons**, each representing a digit from **0** to **9**.
- A **softmax** activation function is applied to provide probabilities for each digit class.

### Flattening the Input
- The input images (28x28 pixels) are flattened into a 1D array of size **728** using the **Flatten** layer in Keras. This is necessary to convert the 2D image data into a shape compatible with the Dense layers.

## 📦 Model Summary

- **Input Shape**: `(28, 28)`
- **Number of Parameters**: 
    - Input to Hidden: 728 x 128 parameters (weights + bias)
    - Hidden to Output: 128 x 10 parameters (weights + bias)
- **Activation Functions**:
    - Hidden Layer: `ReLU`
    - Output Layer: `Softmax`

## 🚀 How to Run the Model

1. Clone the repository:
   ```bash
   git clone https://github.com/Dawood-Imran/Handwritten-Digit-Classification.git
## 🎯 Performance
- The model achieves around 98% accuracy on the test dataset after training for 10 epochs.
