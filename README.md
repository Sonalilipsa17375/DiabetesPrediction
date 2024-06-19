
---

# Diabetes Prediction Model

This project involves training a Support Vector Machine (SVM) model to predict diabetes based on a dataset of medical diagnostic measurements. The process includes data standardization, model training, and saving the predictions to a CSV file.

## Table of Contents
- [Installation](#installation)
- [Usage](#usage)
- [Dataset](#dataset)
- [Model Training](#model-training)
- [Prediction and Output](#prediction-and-output)
- [Results](#results)
- [License](#license)

## Installation

1. Clone the repository:

    ```sh
    git clone https://github.com/Sonalilipsa17375/DiabetesPrediction.git
    cd DiabetesPrediction
    ```

2. Install the necessary packages:

    ```sh
    pip install pandas scikit-learn
    ```

## Usage

1. Ensure you have the dataset (`diabetes.csv`) in the working directory.

2. Run the script to train the model and generate predictions:

    ```sh
    python diabetes_prediction.py
    ```

## Dataset

The dataset used is the Pima Indians Diabetes Database, which is available on Kaggle. The dataset contains several medical diagnostic measurements and a binary outcome indicating the presence or absence of diabetes.

## Model Training

The script performs the following steps to train the model:

1. Load the dataset using pandas.
2. Split the data into features (`X`) and target (`Y`).
3. Standardize the feature data using `StandardScaler`.
4. Split the standardized data into training and testing sets using `train_test_split`.
5. Train an SVM classifier with a linear kernel on the training data.
6. Evaluate the model's accuracy on both the training and testing sets.

## Prediction and Output

After training the model, the script:

1. Makes predictions on the test set.
2. Creates a DataFrame containing the test features and their corresponding predictions.
3. Saves the DataFrame to a CSV file named `submission.csv`.

## Results

The model's performance is evaluated using accuracy scores on the training and testing data. The predictions are saved in `submission.csv`, which includes the test features and their predicted outcomes.
