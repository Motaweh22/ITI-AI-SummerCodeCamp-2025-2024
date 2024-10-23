
---

# Loan Data Analysis

This project focuses on analyzing customer and loan data to uncover insights about gender distribution, age distribution, loan program popularity, original booked amounts, and car types associated with loans. The project uses Python for data processing and visualization with libraries such as `pandas`, `matplotlib`, and `seaborn`.

## Table of Contents
- [Installation](#installation)
- [Data Description](#data-description)
- [Usage](#usage)
- [Features](#features)
- [Contributing](#contributing)
- [License](#license)

## Installation

To run this project, you need to have Python installed along with the following libraries:
- `pandas`
- `matplotlib`
- `seaborn`

You can install the required libraries using:
```bash
pip install pandas matplotlib seaborn
```

## Data Description

The project uses three datasets:
1. **Customers Information** (`customers_info.csv`): Contains information about the customers, such as ID, gender, birth date, and profession.
2. **Labels** (`labels.csv`): Holds labeling information related to the customers.
3. **Loan Information** (`loan_info.csv`): Includes details about the loan, such as loan program name, amount, open date, and expected close date.

## Usage

1. **Merge the Datasets**: The project merges the datasets on `CUSTOMER_ID` and `ACCOUNT_NUMBER` to create a unified dataset.
2. **Data Cleaning**: Redundant columns are dropped, duplicates are removed, date columns are converted to the proper format, and missing values are handled.
3. **Analysis and Visualization**: Several visualizations are created to gain insights from the data:
   - Gender distribution of customers
   - Age distribution of customers
   - Popularity of different loan programs
   - Distribution of original booked loan amounts
   - Top car types associated with loans

### Running the Code

To execute the code, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/loan-data-analysis.git
   ```
2. Navigate to the project directory:
   ```bash
   cd loan-data-analysis
   ```
3. Run the script:
   ```bash
   python loan_data_analysis.py
   ```

Make sure to update the paths in the script to match the location of your datasets.

## Features

1. **Data Merging**: Combines customer and loan information into a single dataset.
2. **Data Cleaning**: Handles missing values and converts date columns.
3. **Visualization**: Uses various plots to display data insights, such as histograms, bar plots, and count plots.

## Contributing

Contributions are welcome! If you want to contribute to this project, follow these steps:

1. Fork the repository.
2. Create a new branch: `git checkout -b feature-branch-name`
3. Commit your changes: `git commit -m 'Add some feature'`
4. Push to the branch: `git push origin feature-branch-name`
5. Open a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

---