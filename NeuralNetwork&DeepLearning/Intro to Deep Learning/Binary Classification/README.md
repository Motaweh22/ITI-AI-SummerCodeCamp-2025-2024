

---

# Hotel Cancellation Prediction

This project is an exercise from the Intro to Deep Learning course. It involves building a binary classifier model to predict hotel cancellations using a dataset that contains various features related to hotel bookings.

## Table of Contents
1. [Introduction](#introduction)
2. [Setup](#setup)
3. [Data Preprocessing](#data-preprocessing)
4. [Model Definition](#model-definition)
5. [Training the Model](#training-the-model)
6. [Results](#results)
7. [Installation](#installation)
8. [Usage](#usage)
9. [License](#license)

## Introduction
In this exercise, you'll build a model to predict hotel cancellations using a binary classifier. The goal is to understand how different factors influence the likelihood of cancellation.

## Setup
To set up the environment for this project, you'll need to install the required libraries. Here are the primary libraries used in this project:

- `numpy`
- `pandas`
- `scikit-learn`
- `tensorflow`
- `matplotlib`

You can install the required libraries using pip:

```bash
pip install numpy pandas scikit-learn tensorflow matplotlib
```

## Data Preprocessing
The dataset used in this project is the Hotel Cancellations dataset, which can be loaded from the specified path. The features are divided into numerical and categorical types and are preprocessed using pipelines that include imputation and scaling for numerical features, and one-hot encoding for categorical features.

### Steps:
1. Load the dataset.
2. Split the data into training and validation sets.
3. Preprocess the features using pipelines.

## Model Definition
The model architecture includes the following layers:

- Batch Normalization
- Dense (Fully Connected) Layers with ReLU activation
- Dropout Layers
- Output Layer with Sigmoid activation

Here's a brief code snippet showing how the model is defined:

```python
from tensorflow import keras
from tensorflow.keras import layers

model = keras.Sequential([
    layers.BatchNormalization(input_shape=input_shape),
    layers.Dense(256, activation='relu'),
    layers.BatchNormalization(),
    layers.Dropout(0.3),
    layers.Dense(256, activation='relu'),
    layers.BatchNormalization(),
    layers.Dropout(0.3),
    layers.Dense(1, activation='sigmoid')
])
```

## Training the Model
The model is compiled using the Adam optimizer and binary cross-entropy loss function. The model is trained with early stopping to avoid overfitting. 

### Training Code:
```python
history = model.fit(
    X_train, y_train,
    validation_data=(X_valid, y_valid),
    batch_size=512,
    epochs=200,
    callbacks=[early_stopping],
)
```

## Results
The model's performance is evaluated using learning curves for cross-entropy loss and accuracy metrics. You can visualize the results using Matplotlib.

```python
history_df = pd.DataFrame(history.history)
history_df.loc[:, ['loss', 'val_loss']].plot(title="Cross-entropy")
history_df.loc[:, ['binary_accuracy', 'val_binary_accuracy']].plot(title="Accuracy")
```

## Installation
Clone this repository and navigate to the project directory:

```bash
git clone <repository_url>
cd hotel-cancellation-prediction
```

## Usage
To run the project, ensure that you have all the dependencies installed and execute the notebook or Python script.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---
