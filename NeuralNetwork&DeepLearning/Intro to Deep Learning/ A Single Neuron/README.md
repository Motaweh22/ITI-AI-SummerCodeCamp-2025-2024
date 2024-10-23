
---

# Wine Quality Prediction using a Linear Model with Keras

This project demonstrates the use of a simple linear neural network model to predict the quality of red wine based on its physiochemical properties. It serves as an introductory exercise in deep learning, covering fundamental concepts such as neural networks, linear regression, and model building with the Keras library.

## Table of Contents

- [Introduction](#introduction)
- [Dataset](#dataset)
- [Project Overview](#project-overview)
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [Explanation of the Code](#explanation-of-the-code)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Introduction

The tutorial introduces the basics of building a neural network model using Keras, starting with a simple linear model. The goal is to predict a wine's perceived quality based on physiochemical measurements. The tutorial covers:
- Setting up the environment and loading the dataset.
- Defining the model structure.
- Understanding model parameters (weights and biases).
- Visualizing the behavior of an untrained linear model.

## Dataset

The dataset used in this project is the **Red Wine Quality** dataset, which contains approximately 1,600 samples of Portuguese red wines. Each sample includes 11 features, such as:
- Fixed acidity
- Volatile acidity
- Citric acid
- Residual sugar
- Chlorides
- Free sulfur dioxide
- Total sulfur dioxide
- Density
- pH
- Sulphates
- Alcohol

The target variable is **quality**, which represents a quality rating based on blind taste tests.

## Project Overview

The project walks through the following steps:

1. **Setup**: Configure plotting styles and import necessary libraries.
2. **Data Exploration**: Load the dataset and inspect its structure.
3. **Model Definition**: Build a linear model using a single dense layer in Keras, suitable for regression tasks.
4. **Examine Model Weights**: Display the initial weights and biases.
5. **Optional Visualization**: Plot the output of the untrained model to understand how random weights affect predictions.

## Requirements

- Python 3.x
- Jupyter Notebook
- Required Python packages:
  - `tensorflow`
  - `pandas`
  - `matplotlib`
  - `numpy`

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/wine-quality-prediction.git
   cd wine-quality-prediction
   ```

2. Install the required packages:
   ```bash
   pip install -r requirements.txt
   ```

## Usage

1. Open the Jupyter Notebook:
   ```bash
   jupyter notebook
   ```

2. Navigate to the notebook file (`wine_quality_prediction.ipynb`) and run the cells sequentially.

## Explanation of the Code

- **Setup**: Sets up plotting configurations and feedback systems.
- **Data Loading**: Uses Pandas to load the Red Wine Quality dataset.
- **Model Definition**: Defines a Keras sequential model with one dense layer.
- **Weights Examination**: Displays the model's randomly initialized weights and biases.
- **Visualization**: Plots the predictions made by the untrained model.

## Results

The initial model output represents a straight line in the plot, corresponding to the random initialization of weights. After training (not included in this tutorial), the model would learn better weights to fit the dataset.

## Contributing

Feel free to submit pull requests or open issues to improve this project. Contributions are welcome!

