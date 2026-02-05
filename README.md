# Malaria Detection in Blood Smears

## Overview
This project focuses on identifying malaria parasites in red blood cell images using **Deep Learning**. The goal is to provide an automated classification tool to support medical diagnosis in high-risk areas.

## 🛠 Methodology
* **Data Prep**: Images loaded with **PIL** and **Pandas**, then normalized (0-1).
* **Augmentation**: Applied rotations and flips using `ImageDataGenerator` to improve robustness.
* **Models**: Comparison of **CNN from Scratch**, **VGG16**, and **ResNet50**.
* **Training**: Optimized using **Early Stopping** and **ReduceLROnPlateau**.



## 📊 Performance Evaluation
The models are evaluated on a test set via:
* **Confusion Matrix**: To identify misclassified samples.
* **Metrics**: Precision, Recall (Sensitivity), and F1-Score.
* **ROC/AUC**: Comparison of overall model performance.



## 🚀 Requirements
* TensorFlow / Keras
* Scikit-learn
* Pandas / NumPy
* PIL (Pillow)
* Matplotlib
