# Multi-Class Weather Classification

A computer vision project that classifies weather images into four categories—**Cloudy, Rain, Shine, and Sunrise**—using a custom CNN and a pretrained VGG-16 transfer learning model.

---

## 1. Project Overview
This project builds and compares two deep learning models to automatically identify the weather condition depicted in an image. It covers the end-to-end pipeline—from raw image ingestion and preprocessing to model training, evaluation, and comparative performance analysis.

---

## 2. Objective
To classify input images into one of four distinct weather categories with high accuracy, while comparing the baseline performance of a **custom-built CNN** against a **VGG-16 model leveraging transfer learning**.

---

## 3. Dataset
* **Name:** Multi-class Weather Dataset
* **Source:** [Kaggle Dataset](https://www.kaggle.com/datasets/pratik2901/multiclass-weather-dataset)
* **Type:** Image Dataset
* **Target Classes (4):** `Cloudy`, `Rain`, `Shine`, `Sunrise`

---

## 4. Features
* **Automated Data Ingestion:** Loads and labels images directly from folder structures.
* **Data Augmentation:** Applies random flips, rotations, and zooms to enhance generalization and mitigate overfitting.
* **Dual Architecture Comparison:** Trains and benchmarks a custom CNN against a pretrained VGG-16 model.
* **Regularization & Early Stopping:** Prevents model overtraining by monitoring validation metrics.
* **Performance Visualization:** Plots learning curves (loss/accuracy) and confusion matrices for direct comparison.

---

## 5. Preprocessing Pipeline
1. **Directory Ingestion:** Load raw images mapped to class-specific folders.
2. **Resizing:** Standardize all images to $128 \times 128$ resolution.
3. **Normalization:** Rescale pixel values from $[0, 255]$ to the range $[0, 1]$.
4. **Data Splitting:** Partition data into **80% Training** and **20% Validation** sets.
5. **Augmentation:** Apply transformations to the training set exclusively.

---

## 6. Tech Stack
* **Language:** Python
* **Deep Learning Framework:** TensorFlow / Keras
* **Data & Math Libraries:** NumPy, Pandas
* **Visualization:** Matplotlib, Seaborn
* **Environment:** Google Colab / Jupyter Notebooks

---

## 7. Instructions to Run

1. **Open in Google Colab:**
   Upload the project notebook (`.ipynb`) to [Google Colab](https://colab.research.google.com/).

2. **Prepare Dataset:**
   * Download the dataset from Kaggle.
   * Upload and extract the dataset folder into your Colab environment or mount your Google Drive.

3. **Install Dependencies:**
   Run the setup cell to install any missing dependencies (if required):
   ```bash
   pip install tensorflow numpy pandas matplotlib seaborn
