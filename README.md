
# Medical AI - Chest X-ray Classification

## Overview

This repository contains code for a binary classification model using transfer learning to classify chest X-ray images. The model is trained to distinguish between images showing the presence of a specific medical condition (e.g., atelectasis) and images with no findings.

## Getting Started

### Prerequisites

- Python 3.x
- TensorFlow 2.x
- NumPy
- Pandas
- Matplotlib
- scikit-learn


## Usage

1. **Data Preparation:**
   - Ensure you have the required dataset (chest X-ray images and labels).
   - Update the `labels.csv` file with image filenames and corresponding labels.

2. **Environment Setup:**
   - Set up a virtual environment and install dependencies.

3. **Training:**
   - Adjust parameters such as learning rate, image dimensions, and model architecture in the code.


4. **Inference:**
   - Use the trained model for image classification.

5. **Results:**
   - View ROC curves, AUC values, and other metrics in the notebook

## Directory Structure

- `medical/images/`: Directory containing chest X-ray images.
- `labels.csv`: CSV file with image filenames and labels.
- `Chestxray.ipynb`: Script for training the classification model.

bui

## Acknowledgments

- This code is based on the [medical-ai](https://github.com/adleberg/medical-ai) repository by [Jason Adleberg](https://github.com/adleberg).

