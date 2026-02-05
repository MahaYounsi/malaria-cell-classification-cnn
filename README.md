# malaria-cell-classification-cnn
Automated Classification of Infected Red Blood Cells for Malaria Diagnosis using CNN.

Project Overview
This project aims to develop and train Convolutional Neural Network (CNN) models to automate the diagnosis of malaria by classifying images of red blood cells (erythrocytes) as either parasitized or uninfected.
The early and accurate detection of this disease is crucial for effective treatment, especially in tropical regions where specialized medical expertise may be limited.

Dataset
The dataset consists of microscopic images of healthy and infected blood cells.
Source: NIH (National Institutes of Health).
Classes: Parasitized and Uninfected.

Methodology
The project follows a rigorous deep learning pipeline:
Data Preprocessing: Images are loaded using PIL and Pandas, normalized to a [1,0] range, and labels are encoded using LabelEncoder.
Data Augmentation: Techniques such as rotations, zooms, and horizontal flips are applied via ImageDataGenerator to improve model generalization.
Model Implementation: Three different CNN architectures are compared:
CNN from Scratch: A Sequential model with Conv2D, MaxPooling, and Dropout layers.
VGG16: Fine-tuning a pre-trained model on ImageNet.
ResNet50: Fine-tuning a pre-trained residual network on ImageNet.
Training Optimization: Implementation of Early Stopping and Learning Rate Decay (ReduceLROnPlateau) to ensure optimal convergence.

Evaluation Metrics
Models are evaluated on a test set using the following metrics:
Confusion Matrix: To visualize classification errors.
Precision, Recall (Sensitivity), and F1-Score.
Specificity: Calculated to assess the ability to identify healthy cells.
ROC Curve & AUC Score: To compare the global performance of the three models.

Requirements
To run this notebook, you need the following libraries:
  tensorflow
  pandas
  numpy
  scikit-learn
  pillow
  matplotlib
