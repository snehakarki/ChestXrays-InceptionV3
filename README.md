
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

##Concepts used
The primary gist of our model is that it uses Transfer Learning to create a convolutional neural network (CNN) model for binary classification based on the InceptionV3 architecture. 

**InceptionV3**
Inception v3 is an image recognition model that has been shown to attain greater than 78.1% accuracy on the ImageNet dataset.One thing that is commonly done in computer vision is that we take a model trained on a very large dataset, then we run it on our own, smaller dataset. We then extract the intermediate representations (features) that the model generates. Even though the task may be quite different from the problem that the original model was trained on, but these representations are frequently informative for our own computer vision task,
The model itself is made up of symmetric and asymmetric building blocks. This includes convolutions, average pooling, max pooling, concatenations, dropouts, and fully connected layers. Batch normalization is used extensively throughout the model and applied to activation inputs. Loss is computed using Softmax.

**Transfer learning**
Transfer learning is beneficial in this context because the InceptionV3 model, which is pre-trained on a large dataset like ImageNet, has already learned useful features for image recognition. By using these pre-trained features, the model can achieve good performance even with a relatively small dataset. Like in this case a smaller dataset which is specific to the current task (detecting cardiomegaly in medical images). This approach is efficient in terms of both computation and data requirements.

**Binary Classification**
Binary classification is a type of machine learning task. Here the goal is to classify input instances into one of two possible classes. In other words, it involves assigning a binary label to each instance based on its characteristics. The two classes are often denoted as positive and negative, or class 1 and class 0. In our model, the binary classification task involves distinguishing between two classes: "cardiomegaly" (positive) and "No Finding" (negative). The data is split into training and testing sets. The images are organized and loaded into memory for visualization. This sets the stage for training a binary classification model.

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



## Acknowledgments

- This code is based on the [medical-ai](https://github.com/adleberg/medical-ai) repository by [Jason Adleberg](https://github.com/adleberg).

