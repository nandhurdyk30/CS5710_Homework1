# CS5710 - Machine Learning  
## Home Work 1  

**Student:** Nandini Reddy
**Course:** CS5710 – Machine Learning  
**Semester:** Spring 2026  

---

## Problem Description

The goal of this assignment is to implement Linear Regression using two different approaches and compare their results:

- Analytical solution using the Normal Equation
- Iterative optimization using Gradient Descent (implemented manually without scikit-learn)

Both methods are applied to the same synthetic dataset to evaluate convergence and parameter estimation.

---

## Data Generation

The dataset was synthetically created using the model:

y = 3 + 4x + ε

where:
- x values are uniformly sampled in the range [0, 5]
- ε represents Gaussian noise
- Total number of samples: 200

A column of ones was added to the feature matrix to incorporate the bias term.

---

## Method 1: Normal Equation

The closed-form solution was computed using:

θ = (XᵀX)⁻¹Xᵀy

This method directly calculates the optimal parameters without iterative updates.

The resulting intercept and slope are displayed in the notebook, along with a regression line plotted against the dataset.

---

## Method 2: Gradient Descent

Gradient Descent was implemented from scratch with the following configuration:

- Initial parameters set to zero
- Learning rate: 0.05
- Total iterations: 1000
- Loss function: Mean Squared Error (MSE)

The algorithm updates parameters iteratively using the gradient of the loss function. A loss curve is plotted to visualize convergence over iterations.

---

## Visual Outputs

The notebook includes:

- Scatter plot of the synthetic dataset
- Regression line using Normal Equation
- Regression line using Gradient Descent
- Combined comparison plot
- Loss vs Iterations graph

---

## Observations

The parameters obtained from Gradient Descent closely match those computed using the Normal Equation. The loss decreases consistently across iterations, demonstrating successful convergence. Both methods produce nearly identical regression lines.

---
