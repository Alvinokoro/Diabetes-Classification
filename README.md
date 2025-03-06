# Diabetes-Classification
Overview
This project implements a logistic regression model from scratch to predict diabetes outcomes based on medical predictors. The model uses gradient descent optimization with L2 regularization and custom implementation of the sigmoid function.

Dataset
The dataset used is the Pima Indians Diabetes Database, which contains several medical predictor variables and one target variable (Outcome):
Predictors: Pregnancies, Glucose, BloodPressure, SkinThickness, Insulin, BMI, DiabetesPedigreeFunction, Age
Target: Outcome (0 = No diabetes, 1 = Diabetes)

Implementation Details
Data Preprocessing:

Split data into features (X) and target (y)
Created train/test split (80/20) using scikit-learn
Applied standardization using sklearn's StandardScaler
Implemented a manual z-score normalization function

Model Components
The logistic regression model includes:

Sigmoid activation function with numerical stability enhancements
Cost function for binary classification with L2 regularization
Gradient computation for weight and bias parameters
Gradient descent optimization algorithm
Prediction function with 0.5 threshold

Key Functions

sigmoid(): Implements the sigmoid activation function with clipping to prevent overflow
compute_cost(): Calculates binary cross-entropy loss with regularization
compute_gradient(): Computes gradients for weight and bias updates
gradient_descent(): Implements the optimization algorithm with learning rate
predict(): Makes binary predictions based on probability threshold

Visualization

Learning curve showing cost function convergence
Actual vs. predicted outcome plot
Confusion matrix visualization

Results
Model performance metrics:
Test accuracy: 0.7532
Detailed performance breakdown via confusion matrix
