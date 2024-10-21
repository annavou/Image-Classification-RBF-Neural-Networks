# Image Classification with RBF NN

This repository implements three different classifiers for solving a binary categorization problem using data from the CIFAR-10 dataset. The classifiers implemented are:

- Radial Basis Function Neural Network (RBF NN)
- Nearest-Neighbor Classifier (k-NN)
- Nearest Centroid Classifier

## Problem Description
We aim to classify images from the airplane and automobile categories of the CIFAR-10 dataset. The CIFAR-10 dataset contains a total of 60,000 color images (32x32 pixels), divided into 10 categories. However, for this project, only the airplane and automobile images will be used:

- Airplane class: 5,000 images
- Automobile class: 5,000 images

Each image in the dataset has 3072 features, represented as a flattened vector of pixel values (32x32x3). To improve efficiency and reduce the dimensionality of the data, we will apply Principal Component Analysis (PCA).

## Classifiers
- **RBF NN**: An RBF neural network with a custom RBF kernel for classifying images into two categories (airplanes and automobiles). It reduces dimensionality using PCA, trains    the model using a binary cross-entropy loss function, and evaluates its accuracy on test data.
- **KNN Classifier**: Implemented using sklearn.neighbors.KNeighborsClassifier. The value of k (number of neighbors) can be adjusted to optimize classification performance.
- **NC Classifier**: Implemented using sklearn.neighbors.NearestCentroid.

## Results
The classifiers will be evaluated on their ability to correctly categorize images as either airplanes or automobiles. The results will include performance metrics such as accuracy, precision, recall, and F1-score.
