# Crop Prediction

This repository contains the code and resources for a machine learning project aimed at predicting the best crops to plant based on various environmental factors.

## Table of Contents

- [Introduction](#introduction)
- [Dataset](#dataset)
- [Features](#features)
- [Model](#model)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Introduction

Crop prediction is essential for optimizing agricultural productivity. By leveraging machine learning techniques, this project aims to predict the most suitable crops for given environmental conditions such as soil type, temperature, and rainfall.

## Dataset

The dataset used in this project includes various environmental parameters that influence crop growth. These parameters include:

- Soil Type
- Temperature
- Rainfall
- pH Level
- Humidity

## Features

The features used for prediction include:

- **Soil Type:** Type of soil (e.g., sandy, loamy, clay)
- **Temperature:** Average temperature in degrees Celsius
- **Rainfall:** Annual rainfall in millimeters
- **pH Level:** Soil pH level
- **Humidity:** Average relative humidity

## Model

We have used several machine learning algorithms to predict the crop suitability, including:

- Decision Trees
- Random Forest
- Support Vector Machine (SVM)
- Neural Networks

The final model is selected based on performance metrics such as accuracy, precision, and recall.

## Installation

To run this project locally, please follow these steps:

1. Clone the repository
    ```bash
    git clone https://github.com/shrushtiGadad/crop-prediction.git
    cd crop-prediction
    ```
3. Install the required dependencies
    ```bash
    pip install -r requirements.txt
    ```

## Usage

1. Ensure you have the dataset in the correct format.
2. Run the data preprocessing script
    ```bash
    python preprocess.py
    ```
3. Train the model
    ```bash
    python train.py
    ```
4. Make predictions
    ```bash
    python predict.py --input data/input_data.csv --output data/output_predictions.csv
    ```

## Results

The results of the model will be saved in the `output_predictions.csv` file. You can view the performance metrics by running:
```bash
python evaluate.py
