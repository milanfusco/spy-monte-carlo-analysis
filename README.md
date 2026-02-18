# SPY Monte Carlo Analysis

## Overview
This project evaluates the adequacy of Geometric Brownian Motion (GBM) as a
structural model for SPY equity returns and assesses the statistical reliability
of Monte Carlo option pricing under the Black–Scholes framework. Simulations are
performed using a purpose-built parallel Monte Carlo engine with reproducible
NumPy Philox random streams.

## Methods
- GBM path simulation via closed-form solution under the real-world measure
- Distributional comparison: historical SPY returns vs. simulated GBM returns
- Hypothesis testing: two-sample z-test, Levene's variance test, Shapiro–Wilk normality test
- Risk-neutral option pricing (European call and put) with put–call parity verification
- Option Greeks estimated via central finite differences

## Results
- Historical SPY returns exhibit excess kurtosis of 19.182, strongly rejecting GBM's Gaussian assumption
- Monte Carlo pricing converges with small standard error (SE ≈ 0.31 for call)
- Structural model error dominates Monte Carlo sampling error

## Technologies
Python · NumPy · SciPy · Matplotlib · yfinance

## Files
| File | Description |
|------|-------------|
| `spy_monte_carlo_analysis.ipynb` | Full analysis notebook with code and outputs |
| `spy_monte_carlo_analysis.pdf` | Rendered notebook as PDF |
| `spy_monte_carlo_analysis_presentation.pdf` | Beamer slide deck |

## Author
Milan Fusco
[github.com/milanfusco](https://github.com/milanfusco)
