# Nearest Neighbor Classifier

## Table of Contents

1. [Introduction](#introduction)
2. [Nearest Neighbor Classifier](#nearest-neighbor-classifier)
3. [Bias, Variance and Generalization](#bias-variance-and-generalization)
4. [Distance Functions](#distance-functions)
5. [K-Nearest Neighbor Classifier](#k-nearest-neighbor-classifier)
6. [Generalization and Cross-Validation](#generalization-and-cross-validation)
7. [Distance Metrics](#distance-metrics)
8. [Summary](#summary)

---

## Introduction

Nearest Neighbor (NN) is a simple and powerful classification algorithm. It works based on the assumption that similar instances are located near each other in the feature space. The most popular example is the **MNIST dataset**, which contains 60,000 training images and 10,000 test images of handwritten digits.

## Nearest Neighbor Classifier

The main idea of the Nearest Neighbor classifier is to assign a class to a data point based on the class of its nearest neighbors in the training set. It relies on the concept of distance metrics to determine the closeness of instances.

### Example:

For MNIST, if a new digit is introduced, the classifier searches for the closest digit in the training set and assigns the label of that nearest digit.

## Bias, Variance and Generalization

* **Bias**: Errors introduced by oversimplified models. High bias can cause underfitting.
* **Variance**: Sensitivity to training data. High variance can cause overfitting.
* **Generalization**: The ability of the model to perform well on unseen data.

### Real-world Analogy:

Imagine studying for a math exam:

* The exercises you practice are like training data.
* The exam problems are like test data.
* If you only memorize the exercises, you may fail to generalize and solve new problems.

## Distance Functions

The choice of distance function (e.g., **Euclidean**, **Manhattan**) impacts the performance of the NN classifier. Different tasks may require different metrics to capture similarity effectively.

### Common Distance Metrics:

* **Euclidean Distance**: Measures the straight-line distance between two points.

  \\\[d(x, y) = \sqrt{(x\_1 - y\_1)^2 + (x\_2 - y\_2)^2}]

  **Example:**
  Consider two points A(1, 2) and B(4, 6). The Euclidean Distance is calculated as:
  \\\[d(A, B) = \sqrt{(4 - 1)^2 + (6 - 2)^2} = \sqrt{9 + 16} = 5]

* **Manhattan Distance**: Measures the distance along grid paths.

  \\\[d(x, y) = |x\_1 - y\_1| + |x\_2 - y\_2|]

* **Minkowski Distance**: A generalized form of both Euclidean and Manhattan.

## K-Nearest Neighbor Classifier

An extension of the NN classifier where instead of the single closest neighbor, the class is determined by a majority vote among the k-nearest neighbors.

### Example:

If $k=3$, the three nearest neighbors are checked, and the most common class among them is selected as the prediction.

```
**Example Visualization:**
- Point X is classified based on the labels of its 3 nearest neighbors (e.g., two are class A and one is class B, so X is assigned to class A).
```

## Generalization and Cross-Validation

To evaluate the model's generalization ability, techniques such as **cross-validation** are used. This helps to assess the performance on unseen data without overfitting.

### Techniques:

* **Holdout Validation**: Divides the data into training and testing sets.
* **k-Fold Cross-Validation**: Splits the data into $k$ parts, trains on $k-1$ and tests on the remaining part, repeated for each fold.
* **Leave-One-Out Cross-Validation**: Extreme case where each instance is tested one by one.

## Distance Metrics

Different distance metrics can be applied:

* Euclidean Distance
* Manhattan Distance
* Minkowski Distance

Each has its advantages depending on the data's structure.

## Summary

The Nearest Neighbor approach is simple yet effective for many classification tasks. It requires no training phase but can be computationally expensive during inference. Choosing the right distance metric and handling bias/variance is key to successful application.

---

Feel free to add more sections or suggest improvements!
