# Regression, Regularization, and Over-Parameterization

This project focuses on exploring key concepts in regression, including data generation, linear model fitting, regularization techniques, and parameterization analysis. I generated a synthetic dataset with structured relationships and noise, then I implemented a linear regression model to predict output values based on input features. The project introduces ridge and lasso regularization methods to demonstrate how penalties on model complexity affect the resulting weights and generalization. Additionally, it examines the effects of under-parameterization (fewer features than data points) and over-parameterization (more features than data points) on model performance. Through each step, I was able to analyze training and testing losses, visualize error trends, and investigate how the size of the training data and regularization strength influence the outcomes. This project integrates programming tasks in Python using PyTorch and encourages critical analysis of regression principles and their practical implications.


## Table of Contents
- [Features](#features)
- [Usage](#usage)
- [Code Structure](#code-structure)
- [Requirements](#requirements)
- [File Output](#file-output)
- [License](#license)
- [Important Note](#important-note)


## Features
- **Data Generation**: 
  - Creation of custom datasets with random noise and structured relationships among features
    
- **Linear Regression**: 
  - Implementation of a linear model with a loss function to minimize squared errors
    
- **Regularization Techniques**:
  - Ridge regression for reducing model complexity and penalizing large weights
  - Lasso regression for feature selection and sparsity

- **Parameterization Analysis**:
  - Impact of under-parameterization (fewer features than data points)
  - Over-parameterization (more features than data points) and its relationship with testing error

- **Visualization**: 
    - Loss and error trends as a function of parameters like regularization strength and feature dimensionality
  

## Usage
1. **Clone the repository**:
   ```bash
   git clone https://github.com/Kobe-Martinez/linear-regression.git
   cd linear-regression

2. **Run the notebook**:
  - Open the `.ipynb` file in Jupyter Notebook or JupyterLab
  - Execute cells sequentially to see the implementation and results

3. Experiment with parameters such as training size, regularization strength (`λ` for ridge and `β` for lasso), and dimensionality to explore the effects on the model


## Code Structure

- **Data Generation**: Functions to generate the input matrix `X` and output `y` using noise and dependencies as specified in the homework

- **Model Implementation**:
  - `linear_model`: Calculates predictions for a given set of weights
  - `loss_function`: Computes the mean squared error between predictions and actual values

- **Regularization**:
  - **Ridge regression**: Adds `λ∑w²` to the loss function to reduce model complexity
  - **Lasso regression**: Adds `β∑|w|` to the loss function for feature selection and sparsity

- **Parameterization Analysis**:
  - Experiments with varying feature dimensions and data sizes
  - Visualization of error trends across configurations


## Requirements

- **Python**: 3.8 or later

- **Required libraries**:
  - `torch`
  - `numpy`
  - `matplotlib`

- **Install dependencies**:
  - `pip install torch numpy matplotlib`
 

## File Output

- **The code generates plots visualizing**:
  - Training and testing loss over iterations
  - Effects of varying `λ` and `β` on ridge and lasso regression
  - Error trends under different parameterization settings
 

## License

This project is licensed under the MIT License. See the LICENSE file for details.


## Important Note

This code is intended for educational purposes only; Use this repository responsibly.
