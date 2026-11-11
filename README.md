# 🩺 Breast Cancer Classification using Deep Learning (ANN)

## 📌 Project Overview
This project builds an *Artificial Neural Network (ANN)* using TensorFlow and Keras to classify breast tumors as either *Malignant (Cancerous)* or *Benign (Non-Cancerous)* based on diagnostic cell nuclei features. 

The goal is to assist in early and accurate tumor detection through deep learning techniques.

---

## 📊 Dataset Information
* *Source:* Breast Cancer Wisconsin (Diagnostic) Dataset (via sklearn.datasets)
* *Total Samples:* 569 patient records
* *Features:* 30 numerical features (mean radius, texture, perimeter, area, smoothness, etc.)
* *Target Classes:* 
  * 0 — Malignant (Cancerous)
  * 1 — Benign (Non-Cancerous)

---

## 🛠️ Tech Stack & Libraries Used
* *Language:* Python
* *Deep Learning Framework:* TensorFlow, Keras
* *Data Processing & Analysis:* NumPy, Pandas, Scikit-Learn (train_test_split, StandardScaler)
* *Data Visualization:* Matplotlib
* *Environment:* Google Colab

---

## 🧠 Model Architecture & Workflow
1. *Data Preprocessing:* Handled feature scaling using StandardScaler to normalize input values, which significantly reduced initial training loss and improved convergence.
2. *Neural Network Structure:*
   * Input Layer: Shape (30,)
   * Flatten Layer: Converts input data into a 1D array
   * Hidden Layer: Dense layer with *20 neurons* and ReLU activation
   * Output Layer: Dense layer with *2 neurons* and Sigmoid activation
3. *Compilation & Training:* Trained for *10 epochs* using the Adam optimizer and sparse_categorical_crossentropy loss function with a 10% validation split.

---

## 📈 Key Results & Performance
* *Training Accuracy:* ~95.8%
* *Validation Accuracy:* ~95.6%
* *Test Data Accuracy:* *96.49%* (Test Loss: 0.1348)
* *Predictive System:* Built an end-to-end inference pipeline using np.argmax() that takes raw patient metrics, scales them, and predicts whether the tumor is Malignant or Benign.

---

## 🚀 How to Run This Project
1. Clone this repository or open Project1.ipynb directly in *Google Colab*.
2. Run all cells sequentially to train the neural network and evaluate test accuracy.
3. Use the predictive system cell at the bottom to test predictions on new patient feature values.
