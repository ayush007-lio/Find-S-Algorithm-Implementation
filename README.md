# Find-S Algorithm Implementation

This repository contains a Python implementation of the **Find-S Algorithm**, a foundational concept learning algorithm in Machine Learning.

## Overview
The Find-S algorithm starts with the most specific hypothesis and generalizes it each time it encounters a positive training example that contradicts its current hypothesis.

## Dataset
The implementation uses the `enjoysport.csv` dataset, which includes attributes like:
* Sky (Sunny, Rainy)
* AirTemp (Warm, Cold)
* Humidity (Normal, High)
* Wind (Strong, Weak)
* Water (Warm, Cool)
* Forecast (Same, Change)

## How It Works
1. Initialize the hypothesis to the most specific possible: `['0', '0', '0', '0', '0', '0']`.
2. For each positive training example:
   - If the attribute value in the example matches the hypothesis, do nothing.
   - If it doesn't match, replace the attribute in the hypothesis with a generic symbol `?`.
3. Output the final maximally specific hypothesis.

## Requirements
* Python 3.x
* Jupyter Notebook

## Usage
1. Ensure `enjoysport.csv` is in the same directory as the notebook.
2. Run the `Lab1 Find S.ipynb` file to see the step-by-step hypothesis generalization.
