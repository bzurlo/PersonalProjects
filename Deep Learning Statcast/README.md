# Dodgers Deep Learning: Extra-Base Hit Prediction

This project uses Statcast data and a neural network to predict whether a Dodgers batted ball will result in an extra-base hit (double, triple, or home run).

## Problem
Predict the probability of an extra-base hit based on batted-ball and game-context features such as launch speed, launch angle, hit distance, count, inning, and batter/pitcher handedness.

## Approach
- Binary classification problem (XBH vs non-XBH)
- Feature engineering from Statcast data
- Neural network model (MLP)

## Model Architecture
- Feedforward neural network (MLPClassifier)
- Hidden layers: (64, 32)
- Activation: ReLU
- Output: Sigmoid probability of extra-base hit
- Preprocessing:
  - Standard scaling (numeric features)
  - One-hot encoding (categorical features)

## Key Features
- Uses real Statcast data via pybaseball
- Produces probability-based predictions (not just classifications)
- Evaluated using ROC-AUC and precision-recall

## Tools
- Python
- scikit-learn
- pybaseball
- pandas / NumPy / matplotlib

## Results
The model identifies high-quality contact events and assigns probabilities of extra-base hits, enabling probabilistic forecasting rather than binary decisions.
