# COIL-20 Handcrafted Feature-Based Object Classification

This repository implements an end-to-end object classification pipeline on the COIL-20 dataset using handcrafted features and classical machine learning methods.

## Overview

The pipeline consists of:

* Image preprocessing
* HOG feature extraction
* Feature standardization
* Dimensionality reduction using PCA and LDA
* Classification using Linear and RBF SVM
* Stratified 5-fold cross-validation
* Confusion matrix analysis

All steps are implemented using scikit-learn Pipelines to ensure proper evaluation and prevent data leakage.

## Dataset

* COIL-20 dataset
* 20 object classes
* 1440 grayscale images
* Controlled background and lighting

## The COIL-20 dataset can be downloaded from:
https://cave.cs.columbia.edu/repository/COIL-20

## Results

| Method           | Accuracy (%) |
| ---------------- | ------------ |
| PCA + Linear SVM | ~94%         |
| PCA + RBF SVM    | ~95%         |
| LDA + Linear SVM | ~96%         |
| LDA + RBF SVM    | ~97%         |

LDA combined with RBF SVM achieves the best performance.

## Tools Used

Python, OpenCV, scikit-image, scikit-learn, NumPy, Matplotlib

## Authors

Gopinath S
Guruprakash M
Gunaseelan L S

License
This project has been developed for academic purposes.
