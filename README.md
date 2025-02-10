Hyperparameter Tuning Process for Fivco’s nnet08 Model

nnet08 is a tool utilizing back propagation and unique regularization to produce a neural net score refined for rare event detection, such as payment card fraud.

Training Process:
Training starts with random weights, with back propagation of errors used to adjust the weights until the network converges.

Model Structure:
The model is typically a single layer, segmented into different parts to represent varying degrees of freedom.

Production Deployment:
In production, once the optimal weights are determined, they are fixed and remain unchanged to drive the highest performance.

The hyperparameter tuning focuses on optimizing the initial weight configuration, regularization parameters, and segmentation of the single-layer structure to achieve convergence and maximize detection performance in rare event scenarios.
