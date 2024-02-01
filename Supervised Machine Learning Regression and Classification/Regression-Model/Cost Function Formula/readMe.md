# Cost Function in Linear Regression

## Overview

The cost function in linear regression is a fundamental concept that measures how well the linear regression model is performing. It quantifies the error between the predicted values and the actual values in the training data. The goal in linear regression is to minimize this cost function.

## Definition

For a linear regression model, the cost function, often denoted as \( J(w, b) \), is defined as:

\[ J(w, b) = \frac{1}{2m} \sum_{i=1}^{m} \left( f_{w,b}(x^{(i)}) - y^{(i)} \right)^2 \]

Where:

- \( m \) is the number of training examples.
- \( x^{(i)} \) is the input feature(s) of the \(i\)-th training example.
- \( y^{(i)} \) is the actual output of the \(i\)-th training example.
- \( f_{w,b}(x^{(i)}) \) is the model's prediction, equal to \( wx^{(i)} + b \).
- \( w \) and \( b \) are the model's parameters (weights and bias).


![]()


## Purpose

- **Error Measurement**: It calculates the difference between the predicted values and the actual values.
- **Model Optimization**: By minimizing the cost function, the model learns the most accurate weights and bias to fit the data.

## Minimization

Minimizing the cost function is achieved through optimization algorithms like Gradient Descent. These algorithms iteratively adjust \( w \) and \( b \) to find the values that result in the lowest possible cost.

## Importance

- **Performance Indicator**: It provides a clear, quantitative measure of how well the model is performing.
- **Guide to Learning**: The process of minimizing the cost function guides the model to learn from the training data.

## Conclusion

The cost function is a critical component in linear regression. Understanding and minimizing this function is key to developing effective linear regression models. By continuously evaluating and minimizing the cost function, the model can be trained to make accurate predictions.

