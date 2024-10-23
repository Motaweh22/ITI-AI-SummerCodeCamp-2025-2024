
---

# Loan Data Prediction

This project aims to predict loan-related outcomes using machine learning techniques. It involves data preprocessing, feature engineering, and training a Decision Tree model to classify the loan data. The process includes handling missing values, encoding categorical variables, and evaluating the model's performance.

## Table of Contents
- [Installation](#installation)
- [Data Description](#data-description)
- [Usage](#usage)
- [Features](#features)
- [Contributing](#contributing)
- [License](#license)

## Installation

To run this project, make sure you have Python installed, along with the following libraries:
- `pandas`
- `scikit-learn`

You can install the required libraries using:
```bash
pip install pandas scikit-learn
```

## Data Description

The project uses a dataset named `merged_data_output.csv`, which is assumed to have the following columns:
- **SEX**: Gender of the customer.
- **PROFESSION**: Customer's profession.
- **CAR_TYPE**: Type of car associated with the loan.
- **ORIGINAL_BOOKED_AMOUNT**: The original amount of the loan.
- **label**: The target variable representing the outcome of the loan.
- Other relevant columns that are used for preprocessing but later removed from the model (e.g., `CUSTOMER_ID`, `ACCOUNT_NUMBER`, date columns).

## Usage

1. **Data Preprocessing**: 
   - Imputation of missing values using appropriate strategies (most frequent for categorical variables, mean for numerical).
   - Label encoding for categorical columns to convert them into numeric format.
   - Irrelevant columns are dropped.

2. **Machine Learning Model**:
   - A Decision Tree classifier is trained on the data to predict the target variable.
   - The data is split into training and testing sets (70% training, 30% testing).
   - Model performance is evaluated using accuracy score and classification report.

### Running the Code

To execute the code, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/loan-data-prediction.git
   ```
2. Navigate to the project directory:
   ```bash
   cd loan-data-prediction
   ```
3. Run the script:
   ```bash
   python loan_data_prediction.py
   ```

Make sure to update the file path to match the location of your `merged_data_output.csv` file.

## Features

1. **Imputation of Missing Values**: Uses different strategies for categorical and numerical data.
2. **Encoding Categorical Variables**: Label encoding for features like gender, profession, car type, etc.
3. **Machine Learning Model Training**: Trains a Decision Tree model on the preprocessed data.
4. **Model Evaluation**: Evaluates the model using accuracy score and classification report.

## Contributing

Contributions are welcome! If you would like to improve the project or add new features, follow these steps:

1. Fork the repository.
2. Create a new branch: `git checkout -b feature-branch-name`
3. Make your changes and commit: `git commit -m 'Add new feature'`
4. Push to your branch: `git push origin feature-branch-name`
5. Open a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

---
