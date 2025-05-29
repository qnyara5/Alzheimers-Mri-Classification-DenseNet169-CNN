# Alzheimer's MRI Image Classification using DenseNet169 and CNN

## Overview
This repository contains the implementation of an image classification model to detect Alzheimer's disease from MRI scans. The model architecture combines:
- **DenseNet169** as the base feature extractor
- Additional **Convolutional Neural Network (CNN)** layers on top to improve classification performance

The goal is to classify MRI images to help in early diagnosis of Alzheimer's disease by leveraging transfer learning with DenseNet169 and further fine-tuning with custom CNN layers.



---

## Dataset
The dataset consists of labeled MRI brain images categorized into:
- No Impairment
- Very Mild Impairment
- Mild Impairment
- Moderate Impairment

Dataset link: [Alzheimer's MRI Dataset](https://www.kaggle.com/datasets/lukechugh/best-alzheimer-mri-dataset-99-accuracy/data)

## Model Formats
The trained model is exported in **three different formats** for flexible deployment:

| Format           | Description                          | Location                  |
|------------------|--------------------------------------|---------------------------|
| `SavedModel`     | Native TensorFlow format             | `/saved_model/`           |
| `TensorFlow.js`  | For running in web browsers          | `/tfjs_model/`            |
| `TFLite`         | For mobile and embedded devices      | `/model.tflite`           |

## Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/your-repo-name.git
cd your-repo-name

# Install required packages
pip install -r requirements.txt
