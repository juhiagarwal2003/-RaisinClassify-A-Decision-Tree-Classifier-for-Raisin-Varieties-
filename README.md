# 🍇 RaisinClassify: A Decision Tree Classifier for Raisin Varieties 🎉

Welcome to **RaisinClassify**—a project that implements a Decision Tree Classifier to differentiate between Kecimen and Besni raisin varieties using morphological features extracted from images. This project leverages the Scikit-learn library for building the model and evaluates its performance through various metrics.

## 📚 Table of Contents

1. [Overview](#overview)
2. [Dataset](#dataset)
3. [Google Colab Setup](#google-colab-setup)
4. [Usage](#usage)
5. [Implementation Details](#implementation-details)
6. [Results](#results)
7. [Contributing](#contributing)
8. [Acknowledgements](#acknowledgements)

## 🏫 Overview

The goal of this project is to classify raisin varieties based on extracted morphological features. With a dataset of 900 raisin images, including 450 samples from both Kecimen and Besni varieties, the classifier aims to achieve high accuracy and precision.

## 📊 Dataset

The dataset consists of images of two raisin varieties, Kecimen and Besni, captured with CVS. Key attributes include:

1. **Area**: Number of pixels within the boundaries of the raisin.
2. **Perimeter**: Distance around the boundaries of the raisin.
3. **MajorAxisLength**: Length of the longest axis on the raisin.
4. **MinorAxisLength**: Length of the shortest axis on the raisin.
5. **Eccentricity**: Measure of the eccentricity of the equivalent ellipse.
6. **ConvexArea**: Number of pixels of the smallest convex shell around the raisin.
7. **Extent**: Ratio of the area of the raisin to the total pixels in the bounding box.
8. **Class**: Kecimen (0) and Besni (1) raisin varieties.

## 🚀 Google Colab Setup

Steps to set up your project in Google Colab:

1. **Open the Colab Notebook**:
   - Create a new notebook in Google Colab.

2. **Clone the Repository**:
   ```python
   !git clone https://github.com/yourusername/RaisinClassify.git
   ```

3. **Install Required Libraries**:
   ```python
   !pip install -r RaisinClassify/requirements.txt
   ```

## 🎉 Usage

Run the notebook and execute each cell to preprocess the data, train the classifier, and evaluate its performance.

## ✨ Implementation Details

- **Data Preprocessing**: The dataset is loaded, missing values are handled, and the target variable is converted to binary.
- **Feature Selection**: Chi-square feature selection is used to evaluate and discard less important features.
- **Model Training**: A Decision Tree Classifier is trained with different criteria, including entropy and log loss.
- **Parameter Tuning**: Grid Search is employed for hyperparameter optimization.

## 🎨 Results

The following results were obtained after implementing the Decision Tree Classifier:

- **Confusion Matrix**:
   ```
   [[94  0]
    [ 0 86]]
   ```
- **Accuracy**: 1.0
- **Precision**: 1.0
- **Recall**: 1.0

After tuning the hyperparameters, the best model was achieved with the following parameters:
- **Max Depth**: 10
- **Min Samples Split**: 4
- **Max Features**: 'sqrt'

The optimized model yielded:
- **Best Model - Accuracy**: 1.0
- **Best Model - Precision**: 1.0
- **Best Model - Recall**: 1.0

## 🤝 Contributing

Contributions are welcome! Feel free to open an issue or submit a pull request.

## 🎉 Acknowledgements

- [Scikit-learn](https://scikit-learn.org/stable/)
- UCI Machine Learning Repository for the Raisin Dataset

---

