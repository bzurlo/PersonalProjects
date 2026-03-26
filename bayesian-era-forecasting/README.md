# Bayesian Hierarchical ERA Forecasting

This project uses a Bayesian hierarchical model to estimate and forecast pitcher ERA while accounting for sample size and noise.

## Problem
Observed ERA can be misleading, especially for pitchers with low innings pitched. This project estimates true pitcher talent and produces probabilistic forecasts.

## Approach
- Hierarchical Bayesian model
- League-level distribution (mu, sigma)
- Pitcher-level latent true ERA
- Observation noise scaled by innings pitched
- Inference via MCMC (NUTS sampler)

## Key Features
- Partial pooling (shrinkage toward league mean)
- Posterior inference for pitcher skill
- Probabilistic forecasting
- Uncertainty quantification

## Tools
- PyMC
- pandas / NumPy
- Matplotlib
