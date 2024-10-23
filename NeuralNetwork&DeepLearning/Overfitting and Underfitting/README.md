

---

# Deep Learning Exercise: Early Stopping for Overfitting Prevention

This repository contains a deep learning exercise that demonstrates how to improve model training outcomes by utilizing an early stopping callback to prevent overfitting. The task involves predicting the popularity of a song based on various audio features using a neural network.

## Table of Contents
1. [Introduction](#introduction)
2. [Dataset](#dataset)
3. [Requirements](#requirements)
4. [Installation](#installation)
5. [Usage](#usage)
6. [Project Structure](#project-structure)
7. [Explanation](#explanation)
8. [Results](#results)
9. [Contributing](#contributing)
10. [License](#license)

## Introduction
In this exercise, we predict the popularity of songs using audio features such as 'tempo,' 'danceability,' and 'mode.' By building and training neural networks, we explore ways to improve training outcomes and prevent overfitting using the early stopping technique.

## Dataset
The dataset used is a **Spotify dataset**, containing information about various songs and their features:
- **Features**: `danceability`, `energy`, `key`, `loudness`, `mode`, `speechiness`, `acousticness`, `instrumentalness`, `liveness`, `valence`, `tempo`, `duration_ms`.
- **Target**: `track_popularity`, a numerical value representing the popularity of a song.

The dataset is split into training and validation sets, ensuring that all of an artist's songs appear in only one split to prevent data leakage.

## Requirements
The code uses the following libraries:
- Python 3.x
- pandas
- scikit-learn
- tensorflow
- matplotlib
- seaborn

## Installation
1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/deep-learning-early-stopping.git
   cd deep-learning-early-stopping
   ```
2. **Install the required packages**:
   ```bash
   pip install -r requirements.txt
   ```

## Usage
1. **Prepare the environment**:
   - Run the setup code to configure plotting and initialize the feedback system.
2. **Load the Spotify dataset**:
   - The dataset should be located in the specified directory (`../input/dl-course-data/spotify.csv`).
3. **Preprocess the data**:
   - Standardize numerical features and encode categorical features.
   - Split the dataset into training and validation sets using `GroupShuffleSplit`.
4. **Train the model**:
   - Start with a simple linear model, then add more layers to increase model capacity.
   - Use early stopping to halt training when the validation loss stops improving.
5. **Plot learning curves**:
   - Visualize training and validation losses to understand model performance.

## Project Structure
```
deep-learning-early-stopping/
│
├── data/                         # Contains the dataset (not included in the repository)
├── notebooks/                    # Jupyter notebooks for the exercise
├── README.md                     # This README file
└── requirements.txt              # List of required packages
```

## Explanation
The key steps in this project are:
1. **Model Initialization**: Define the architecture of the neural network using Keras' `Sequential` model.
2. **Model Compilation**: Use the Adam optimizer and mean absolute error (MAE) as the loss function.
3. **Early Stopping Callback**: Add early stopping to prevent overfitting by monitoring validation loss.
4. **Training the Model**: Train the model on the training set and evaluate on the validation set.

## Results
The learning curves show the effect of different model architectures on training outcomes. Adding early stopping significantly reduces the risk of overfitting and helps improve the model's generalization ability.

## Contributing
Contributions are welcome! Feel free to submit a pull request or open an issue if you find a bug or have a suggestion.

## License
This project is licensed under the MIT License.

---

