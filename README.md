# 🧠 Brain Cancer Classification Project

This project uses the [Multi-Cancer Dataset](https://www.kaggle.com/datasets/obulisainaren/multi-cancer) to classify brain cancer images into various types. The dataset includes medical imaging data, and a Convolutional Neural Network (CNN) was developed to achieve high classification accuracy.

---

## 📊 Dataset Overview

The dataset contains images of brain cancer classified into the following categories:

| **Path**             | **Subclass**       | **Description**                      |
|-----------------------|--------------------|--------------------------------------|
| `/brain_glioma`      | Glioma            | Most common brain tumor              |
| `/brain_menin`       | Meningioma        | Tumors affecting brain membranes     |
| `/brain_tumor`       | Pituitary Tumor   | Tumors affecting the pituitary gland |

### Preprocessing
- **Image Size**: Resized to **512x512 pixels**.
- **Normalization**: Pixel values scaled between 0 and 1.
- **Augmentation**:
  - Rotation: ±10°
  - Width/Height Shift: ±10%
  - Shearing/Zooming: ±10%
  - Brightness Adjustment: 20%-120%
  - Horizontal Flip: Randomly flips images for diversity.

---

## 🚀 Model Architecture

A custom Convolutional Neural Network (CNN) was designed for this project:
- **Input Size**: `(512, 512, 3)`
- **Architecture**:
  - Convolutional and pooling layers for feature extraction.
  - Dropout layers for regularization.
  - Dense layers for final classification.

### Model Summary
- **Output Classes**: `3` (Glioma, Meningioma, Pituitary Tumor)
- **Optimization**: Adam optimizer with learning rate scheduling.
- **Loss Function**: Categorical Cross-Entropy.

---

## 📈 Results

| **Metric**           | **Value**          |
|-----------------------|--------------------|
| Validation Accuracy   | **99.2%**         |
| Test Accuracy         | **98.9%**         |
| Precision             | **99.0%**         |
| Recall                | **99.0%**         |
| F1-Score              | **99.0%**         |

### Training and Validation
- **Training Accuracy**: **99.7%**
- **Validation Loss**: **0.0326**

### Training & Validation Curves
Detailed training and validation accuracy/loss trends are included in the notebook. Grad-CAM visualizations are also provided to interpret the model’s decision-making.

