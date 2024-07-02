# Portfolio VaR Calculation using Variance-Covariance, Historical, and Monte Carlo Simulation Methods

This repository contains a Jupyter Notebook for calculating the Value at Risk (VaR) of a portfolio using three different methods: Variance-Covariance, Historical, and Monte Carlo Simulation. The project demonstrates how to estimate the potential loss in portfolio value over a specified time period and at various confidence levels.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [Code Description](#code-description)
- [Results](#results)
- [License](#license)

## Introduction

Value at Risk (VaR) is a statistical measure used to assess the level of financial risk within a portfolio over a specific time frame. This project demonstrates three different methods to calculate VaR:
- Variance-Covariance Method
- Historical Simulation Method
- Monte Carlo Simulation Method

## Features

- Calculation of daily returns from stock price data
- Portfolio VaR calculation using Variance-Covariance method
- Portfolio VaR calculation using Historical method
- Portfolio VaR calculation using Monte Carlo simulation method
- Visualization of portfolio return distribution and VaR

## Requirements

- Python 3.6 or higher
- pandas
- numpy
- matplotlib
- scipy
- statsmodels

## Installation

1. Clone the repository:
   ```sh
   git clone https://github.com/your-username/portfolio-var-calculation.git
   cd portfolio-var-calculation

2. Install the required packages:
pip install -r requirements.txt

Usage
Open the Jupyter Notebook file Portfolio VaR_CoVaR,Hstoorical and Monte Carlo Simulation Method.ipynb.
Run the cells sequentially to calculate and visualize the VaR using different methods.
Code Description
1. Data Preparation
The code starts by loading stock price data into a pandas DataFrame and calculating the daily returns for each stock.

2. Portfolio VaR Calculation using Variance-Covariance Method
Calculate the mean and standard deviation of the portfolio returns.
Determine the z-scores for the desired confidence levels.
Calculate the VaR using the formula:
VaR = μp + z * σp
Where:
μp is the mean (expected) return of the portfolio.
z is the z-score corresponding to the desired confidence level (from the standard normal distribution).
σp is the standard deviation of the portfolio returns.
3. Portfolio VaR Calculation using Historical Method
Sort the historical returns.
Determine the return corresponding to the desired confidence level.
Calculate the VaR using the formula:
VaR = Percentile(returns, (1 - confidence level) * 100)
Where:
Percentile(returns, x) is the x-th percentile of the historical returns.
4. Portfolio VaR Calculation using Monte Carlo Simulation
Simulate portfolio returns using a multivariate normal distribution.
Calculate the VaR from the simulated returns.
Calculate the VaR using the formula:
VaR = Percentile(simulated returns, (1 - confidence level) * 100)
Where:
Percentile(simulated returns, x) is the x-th percentile of the simulated returns.
5. Visualization
The code includes several plots to visualize the distribution of returns and the calculated VaR at different confidence levels.

Results
The results section of the notebook includes the calculated VaR values at different confidence levels for each method. The plots show the distribution of returns and the VaR lines for better visualization.

License
This project is licensed under the MIT License - see the LICENSE file for details


