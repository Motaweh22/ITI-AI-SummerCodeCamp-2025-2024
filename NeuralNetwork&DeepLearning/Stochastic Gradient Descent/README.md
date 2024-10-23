
---

# Deep Learning Intro: Fuel Economy Prediction

This notebook is part of the "Intro to Deep Learning" course. It contains exercises to train a neural network to predict the fuel economy of automobiles based on a dataset of vehicle features. Through this notebook, you will learn to set up a deep learning model, train it with various parameters, and explore how different configurations affect the learning process.

## Overview

The notebook walks through the following steps:
1. **Setup:** Imports the necessary libraries for data processing, model building, and visualization.
2. **Data Loading and Preprocessing:** 
   - Loads the Fuel Economy dataset.
   - Splits the data into features (`X`) and target (`y`).
   - Preprocesses the features using scaling and one-hot encoding.
3. **Model Definition:**
   - Builds a neural network using TensorFlow’s Keras API.
   - Configures a multi-layer perceptron model with three hidden layers.
4. **Model Compilation and Training:**
   - Compiles the model with the Adam optimizer and Mean Absolute Error (MAE) as the loss function.
   - Trains the model on the dataset for 200 epochs with a batch size of 128.
5. **Evaluation and Analysis:**
   - Visualizes the loss curve to assess model performance during training.
   - Discusses the potential benefits of longer training based on the loss curve.
6. **Learning Rate and Batch Size Exploration:**
   - Experiments with different learning rates and batch sizes.
   - Observes how these parameters impact the model’s convergence, training speed, and stability.
7. **Interactive Learning:**
   - Animates the effect of learning rate, batch size, and number of examples on the training of a simple linear model.

## Requirements
The following libraries are required:
- Python 3.x
- TensorFlow
- scikit-learn
- Matplotlib
- Pandas
- Numpy

## How to Use This Notebook
1. **Clone or download** the notebook and place it in an environment with the required libraries installed.
2. **Run the cells sequentially** to follow along with the exercises and learning objectives.
3. **Modify parameters** such as learning rate, batch size, and number of epochs to observe different training behaviors.

## Key Concepts
- **Neural Networks:** Training a neural network to predict continuous values.
- **SGD (Stochastic Gradient Descent):** Observing the impact of batch size and learning rate on training dynamics.
- **Data Preprocessing:** Scaling and encoding data for machine learning.
- **Model Evaluation:** Using loss curves to evaluate training performance.

## Learning Objectives
By the end of this notebook, you will:
- Understand how to preprocess a dataset for deep learning tasks.
- Learn to configure and compile a neural network using TensorFlow's Keras API.
- Gain insights into the effects of training parameters such as batch size and learning rate on model performance.
- Develop skills to visualize and interpret loss curves for model evaluation.

## References
For further details, refer to the tutorial linked within the course.

---
