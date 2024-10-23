
---

# Deep Learning Exercises: Neural Network with Hidden Layers

This notebook is part of the **Intro to Deep Learning** course exercises, focusing on building and experimenting with deep neural networks. In this exercise, we explore the use of activation functions in hidden layers and construct a neural network to predict the compressive strength of concrete.

## Table of Contents

- [Introduction](#introduction)
- [Dataset](#dataset)
- [Project Overview](#project-overview)
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [Explanation of the Code](#explanation-of-the-code)
- [Contributing](#contributing)
- [License](#license)

## Introduction

In this exercise, we learn to build a neural network with multiple hidden layers and experiment with different activation functions beyond ReLU. By stacking layers in a Sequential model and adding activation functions after the hidden layers, the network can learn complex, non-linear relationships in the data.

The task is to predict the compressive strength of concrete based on various input features using a deep learning model built with TensorFlow and Keras.

## Dataset

The dataset used in this exercise is the **Concrete Compressive Strength** dataset, which includes the following features:

- Cement
- Blast Furnace Slag
- Fly Ash
- Water
- Superplasticizer
- Coarse Aggregate
- Fine Aggregate
- Age (days)

The target variable is **CompressiveStrength**, representing the compressive strength of the concrete.

## Project Overview

The project consists of the following steps:

1. **Setup**: Configure the environment and import necessary libraries.
2. **Data Loading**: Load the dataset to be used for training the neural network.
3. **Define Input Shape**: Specify the shape of the input data.
4. **Build the Model**: Create a neural network model with three hidden layers and explore different ways to use activation functions.
5. **Activation Function Alternatives**: Experiment with various activation functions beyond ReLU, such as ELU, SELU, and Swish, and visualize their behavior.

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
   git clone https://github.com/your-username/deep-learning-exercises.git
   cd deep-learning-exercises
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

2. Navigate to the notebook file (`deep_learning_exercise.ipynb`) and run the cells sequentially to follow along with the exercise.

## Explanation of the Code

- **Setup**: Configure plotting styles and set up a feedback system for the course.
- **Data Loading**: Use Pandas to load the Concrete Compressive Strength dataset.
- **Define Input Shape**: Determine the input shape required for the model.
- **Build the Model**: Create a Sequential model with three hidden layers (each having 512 units with ReLU activation) and an output layer for regression.
- **Use Activation Layers**: Demonstrate how to apply activation functions separately using `Activation` layers.
- **Experiment with Activation Functions**: Visualize various activation functions and their effects on input data.

## Contributing

Contributions are welcome! Feel free to open issues, submit pull requests, or suggest features to improve this project.

