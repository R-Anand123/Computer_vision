Multi-Class Weather Classification
A computer vision project that classifies weather images into four categories — Cloudy, Rain, Shine, and Sunrise — using a custom CNN and a VGG-16 transfer learning model.

1. Project Overview
This project builds and compares two deep learning models to automatically identify the weather condition shown in an image. It covers the full pipeline — from raw images to a trained, evaluated model.

2. Objective
To classify a given image into one of four weather categories with high accuracy, and to compare the performance of a custom-built CNN against a pretrained VGG-16 model using transfer learning.

3. Dataset
Dataset: Multi-class Weather Dataset

Source: Kaggle 
Type: Image dataset
Target Variable: Weather Type (Cloudy, Rain, Shine, Sunrise)
Link: https://www.kaggle.com/datasets/pratik2901/multiclass-weather-dataset
4. Features
Automatic image loading and labeling from folder structure
Data augmentation (flip, rotation, zoom) to reduce overfitting
Two model architectures for comparison: custom CNN and VGG-16 transfer learning
Training with early stopping to prevent overfitting
Accuracy comparison and visualization of results
5. Preprocessing Pipeline
Load images from class folders
Resize all images to a fixed size (128×128)
Normalize pixel values to the range [0, 1]
Split data into training and validation sets (80/20)
Apply data augmentation to the training set only
6. Technology Used
Python
TensorFlow / Keras
NumPy, Pandas
Matplotlib
Google Colab
7. Instructions to Run the Project
Open the project notebook in Google Colab.

Upload the Weather dataset (image folders) to the Colab session.
Install the required libraries (if they are not already available).
Run all the notebook cells sequentially.
The notebook will:
Load the dataset
Perform preprocessing (resizing, normalization)
Apply data augmentation
Build and train the custom CNN model
Build and train the VGG-16 transfer learning model
Evaluate and compare both models' accuracy
8. Contributors
Anand
Meenakshi
9. License
This project is for educational purposes only
