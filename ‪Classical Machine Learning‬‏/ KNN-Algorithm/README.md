

---

# Diabetes Dataset KNN Regression Analysis

This project applies K-Nearest Neighbors (KNN) Regression to predict diabetes disease progression using the diabetes dataset. It involves preprocessing the data, generating polynomial features, training a KNN model, and evaluating its performance. The aim is to predict the progression of diabetes based on various health metrics.

## Table of Contents
- [Installation](#installation)
- [Dataset](#dataset)
- [Project Overview](#project-overview)
- [Usage](#usage)
- [Features](#features)
- [Contributing](#contributing)
- [License](#license)

## Installation

To run this project, make sure you have Python installed along with the necessary libraries:
- `numpy`
- `matplotlib`
- `scikit-learn`

Install the libraries using:
```bash
pip install numpy matplotlib scikit-learn
```

## Dataset

The project utilizes the `load_diabetes` dataset from the `sklearn` library. This dataset provides information on diabetes disease progression based on ten baseline health indicators such as age, sex, body mass index, blood pressure, and others.

## Project Overview

The project performs the following steps:

1. **Data Splitting**: The dataset is split into training (80%) and testing (20%) sets.
2. **Feature Scaling**: The features are standardized to improve the model's accuracy, as KNN is sensitive to feature scaling.
3. **Polynomial Feature Expansion**: Polynomial features of degree 2 are generated to capture potential non-linear relationships.
4. **KNN Regression**: A KNN model is trained to predict the target variable using the training data.
5. **Model Evaluation**: The model's performance is assessed using Mean Squared Error (MSE) and R² Score.

## Usage

To execute the code:

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/diabetes-knn-regression.git
   ```
2. Navigate to the project directory:
   ```bash
   cd diabetes-knn-regression
   ```
3. Run the script:
   ```bash
   python diabetes_knn_regression.py
   ```

The code performs the following tasks:
- Loads the diabetes dataset.
- Splits the data into training and testing sets.
- Scales the features using `StandardScaler`.
- Expands the features using `PolynomialFeatures` with a degree of 2.
- Trains a KNN Regression model to make predictions on the test set.
- Evaluates the model using MSE and R² Score.
- Optionally, you can visualize the results with a True vs Predicted plot and a Residuals plot.

## Features

1. **Feature Scaling**: Uses `StandardScaler` to standardize feature values.
2. **Polynomial Transformation**: Adds polynomial features to capture non-linear relationships.
3. **KNN Regression**: Applies K-Nearest Neighbors Regression with customizable parameters such as `n_neighbors`.
4. **Model Evaluation**: Outputs Mean Squared Error and R² Score for performance measurement.
5. **Visualization**:
   - **True vs Predicted Plot**: Shows how well the model's predictions match the actual target values.
   - **Residuals Plot**: Displays residuals to help identify patterns indicating possible model issues.

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

