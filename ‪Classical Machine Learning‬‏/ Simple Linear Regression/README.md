
---

# Diabetes Dataset Regression Analysis

This project performs regression analysis on the diabetes dataset using Ridge Regression with polynomial features. It involves data preprocessing, feature scaling, polynomial transformation, and model evaluation. The goal is to predict diabetes disease progression based on various health factors.

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
- `numpy`
- `matplotlib`
- `scikit-learn`

Install the libraries using:
```bash
pip install numpy matplotlib scikit-learn
```

## Dataset

The project uses the built-in `load_diabetes` dataset from the `sklearn` library. The dataset contains information on diabetes disease progression based on 10 baseline variables such as age, sex, body mass index, blood pressure, and others.

## Project Overview

The project performs the following steps:

1. **Data Splitting**: The dataset is split into training (80%) and testing (20%) sets.
2. **Feature Scaling**: Standardizes the feature values for better model performance.
3. **Polynomial Feature Expansion**: Generates polynomial features to increase the model's complexity and capture non-linear relationships.
4. **Ridge Regression**: Uses Ridge Regression for prediction, which helps avoid overfitting by applying a penalty to the coefficients.
5. **Model Evaluation**: The model's performance is evaluated using Mean Squared Error (MSE) and R² Score.

## Usage

To execute the code:

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/diabetes-regression-analysis.git
   ```
2. Navigate to the project directory:
   ```bash
   cd diabetes-regression-analysis
   ```
3. Run the script:
   ```bash
   python diabetes_regression_analysis.py
   ```

The code performs the following tasks:
- Loads the diabetes dataset.
- Splits the data into training and testing sets.
- Scales the features using `StandardScaler`.
- Expands the features using `PolynomialFeatures` with a degree of 2.
- Fits a Ridge Regression model and makes predictions on the test set.
- Evaluates the model using MSE and R² score.
- Plots the True vs Predicted values and a residuals plot for error analysis.

## Features

1. **Feature Scaling**: Uses `StandardScaler` to standardize feature values.
2. **Polynomial Transformation**: Creates polynomial features to capture non-linear relationships.
3. **Ridge Regression**: Regularized linear regression model that prevents overfitting.
4. **Model Evaluation**: Outputs Mean Squared Error and R² Score to measure model performance.
5. **Visualization**:
   - **True vs Predicted Plot**: Compares the model's predictions against the actual target values.
   - **Residuals Plot**: Shows the residuals to detect patterns that indicate model issues.

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

