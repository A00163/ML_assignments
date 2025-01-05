# KNN Classifier Implementation

This project implements a simple **K-Nearest Neighbors (KNN)** classifier from scratch without using any pre-built libraries for the algorithm. The classifier is used to predict the species of flowers based on their features.

## Features
- Manual implementation of the KNN algorithm.
- Calculates Euclidean distances to find the `k` nearest neighbors.
- Supports both training and testing datasets.
- Generates scatter plots for visualizing the data.

## Files
- `train.csv`: Training dataset.
- `test.csv`: Testing dataset.
- `result.csv`: Output file containing predictions for the test dataset.

## How to Use
1. Upload the training and testing datasets (`train.csv` and `test.csv`) to the `/content/input/` directory.
2. Run the `knn.py` script in Google Colab or any Python environment.
3. The predictions will be saved in `/content/output/result.csv`.

## Requirements
- Python 3.x
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn

## Example Output
- **Training Accuracy**: Displays the accuracy of the model on the training dataset.
- **Test Accuracy**: Displays the accuracy of the model on the test dataset.
- **Scatter Plots**: Visualizes the Sepal Length vs. Sepal Width for both training and test datasets.

## How it Works
1. The `fit` method stores the training data.
2. The `predict_instance` method calculates the Euclidean distances and predicts the label for a single instance.
3. The `predict` method predicts labels for all test instances.
4. Accuracy is calculated using `sklearn.metrics.accuracy_score`.

