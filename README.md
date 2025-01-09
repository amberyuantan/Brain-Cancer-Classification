# Brain Cancer Classification

This project implements a deep learning-based approach to classify brain cancer images. Using convolutional neural networks (CNNs), the model is trained on medical imaging data to predict brain cancer categories with high accuracy.

---

## Project Overview

- **Objective**: Classify brain cancer images into predefined categories using CNNs.
- **Dataset**: Medical imaging dataset containing labeled brain cancer scans.
- **Model**: A custom-built CNN for image classification, with potential for extension to transfer learning models like ResNet or EfficientNet.

---

## Features

- **Data Preprocessing**:
  - Normalization of pixel values.
  - Data augmentation to improve model generalization.
- **Model Architecture**:
  - Built a CNN model with multiple convolutional and pooling layers.
  - Dropout layers for regularization.
- **Evaluation**:
  - Metrics include accuracy, precision, recall, and F1-score.
  - Visualization of training/validation loss and accuracy trends.
- **Visualization**:
  - Heatmaps and confusion matrices to analyze classification results.

---

## Requirements

To run this project, you need the following Python libraries:
- `tensorflow`
- `numpy`
- `matplotlib`
- `seaborn`
- `pandas`
- `scikit-learn`

Install the dependencies using:
```bash
pip install -r requirements.txt
