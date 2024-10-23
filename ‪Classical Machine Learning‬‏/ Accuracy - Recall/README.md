

---

# Iris Dataset KNN Classification

This project performs classification analysis on the Iris dataset using the K-Nearest Neighbors (KNN) algorithm. It involves data preprocessing, model training, and evaluation using a confusion matrix and classification report. The goal is to classify iris flowers into one of three species based on various features.

## Table of Contents
- [Installation](#installation)
- [Dataset](#dataset)
- [Project Overview](#project-overview)
- [Usage](#usage)
- [Features](#features)
- [Contributing](#contributing)
- [License](#license)

## Installation

To run this project, ensure you have Python installed along with the required libraries:
- `pandas`
- `scikit-learn`

Install the libraries using:
```bash
pip install pandas scikit-learn
```

## Dataset

The project uses the Iris dataset from the `sklearn` library. This dataset consists of 150 samples from three species of iris flowers (Setosa, Versicolour, and Virginica). Each sample contains four features: sepal length, sepal width, petal length, and petal width.

## Project Overview

The project performs the following steps:

1. **Data Loading**: The Iris dataset is loaded with features and target labels.
2. **Data Splitting**: The dataset is divided into training (70%) and testing (30%) sets.
3. **Model Training**: A KNN classifier with `k=3` is trained using the training set.
4. **Prediction**: The trained model makes predictions on the test set.
5. **Model Evaluation**: The performance is evaluated using a confusion matrix and classification report.

## Usage

To execute the code:

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/iris-knn-classification.git
   ```
2. Navigate to the project directory:
   ```bash
   cd iris-knn-classification
   ```
3. Run the script:
   ```bash
   python iris_knn_classification.py
   ```

The script performs the following tasks:
- Loads the Iris dataset.
- Splits the data into training and testing sets.
- Trains a KNN classifier on the training data.
- Makes predictions on the test set.
- Evaluates the model's performance using a confusion matrix and a classification report.

## Features

1. **Data Splitting**: Uses `train_test_split` to create training and testing datasets.
2. **KNN Classification**: Applies K-Nearest Neighbors Classification with a customizable number of neighbors (`k=3`).
3. **Model Evaluation**:
   - **Confusion Matrix**: Provides insights into the model's performance across different classes.
   - **Classification Report**: Displays precision, recall, and F1-score for each class.

## Contributing

Contributions are welcome! To contribute:
1. Fork the repository.
2. Create a new branch: `git checkout -b feature-branch-name`
3. Commit your changes: `git commit -m 'Add new feature'`
4. Push the branch: `git push origin feature-branch-name`
5. Open a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

---
