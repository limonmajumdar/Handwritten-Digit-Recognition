# Handwritten-Digit-Recognition
Handwritten Digit Recognition project using the MNIST dataset. This project preprocesses image data, reduces dimensionality with PCA, and classifies digits using an SVM classifier. Includes hyperparameter tuning, model evaluation, and deployment using joblib.


Objective:
The project aims to develop a machine learning model capable of accurately classifying handwritten digits (0-9) from the MNIST dataset. This task is a classic benchmark in machine learning and pattern recognition, often used to test classification algorithms and preprocessing techniques.

Key Components:
Dataset:

MNIST Handwritten Digits: A widely-used dataset consisting of 70,000 grayscale images of handwritten digits.
Each image is 28×28
28×28 pixels, resulting in 784 features (flattened pixel values).
Labels (0–9) correspond to the digit in each image.
Dataset is already pre-labeled and split into training and test sets.
Methods and Techniques:

Data Preprocessing:
Normalization: Scaling pixel values to the range [0, 1] for computational efficiency and faster convergence.
Dimensionality Reduction: Applying PCA to reduce the dataset's dimensionality while retaining 95% of the variance, optimizing computational performance.
Classification Algorithm:
Support Vector Machine (SVM): Leveraging the RBF kernel for non-linear classification to separate complex digit patterns.
Model Optimization:
Hyperparameter tuning using GridSearchCV to identify the best combination of SVM parameters (C, gamma, kernel).
Evaluation Metrics:

Accuracy: Measures the overall percentage of correct predictions.
Confusion Matrix: Evaluates performance by showing true and false positives/negatives for each digit.
Classification Report: Provides precision, recall, and F1-score for each class.
Model Deployment:

The trained SVM model is serialized and saved for future use using the joblib library.
Deliverables:
A functional SVM-based digit recognition model.
Evaluation metrics showing the model's performance.
A saved, deployable model file for reuse.
Potential Applications:
Optical Character Recognition (OCR) systems.
Automated form processing.
Digital document scanning and archiving.
This project demonstrates the application of machine learning for real-world image recognition tasks and serves as a foundation for more complex deep learning models like CNNs in the future.
