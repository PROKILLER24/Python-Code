Tradexa Assignment: Fund Analysis


Date: December 2025

Overview

This repository contains the Jupyter Notebook and PDF for the Tradexa assignment.
The assignment involves analyzing mutual fund data to:

Identify the ideal combination of Market Cap, Type, and Risk that gives the highest 3-Year Return (%).

Analyze the Sharpe Ratio to determine the value that maximizes 1-Year Return (%).

Note: A synthetic dataset was created for demonstration purposes.

Folder Structure
/Tradexa_Assignment
│
├─ Tradexa_Assignment.ipynb   # Jupyter Notebook with full analysis
├─ Tradexa_Assignment.pdf      # PDF export of the notebook
├─ fund_data.csv               # Sample dataset used
└─ README.md                  # This file

Environment Setup

Python Version: 3.12

Libraries Used:

pandas

matplotlib

seaborn

scikit-learn

Setup Commands:

# Create virtual environment
python3 -m venv ~/jupyter-env

# Activate environment
source ~/jupyter-env/bin/activate

# Install libraries
pip install pandas matplotlib seaborn scikit-learn jupyter

# Start Jupyter
jupyter notebook

Dataset
FundName	MarketCap	Type	Risk	SharpeRatio	1YrReturn%	3YrReturn%
Alpha Equity Fund	Large	Equity	High	1.2	18.5	14.2
Bluechip Growth Fund	Large	Equity	Moderate	1.0	15.3	12.8
Midcap Opportunities	Mid	Equity	High	1.4	22.1	17.6
...	...	...	...	...	...	...
Analysis Steps
Step 1: Load Dataset

Load the CSV file into pandas DataFrame and inspect the data.

Step 2: 3-Year Return Analysis

Group by MarketCap, Type, and Risk

Find combination with maximum 3YrReturn%

Visualize using bar plots with matplotlib/seaborn

Step 3: 1-Year Return vs Sharpe Ratio

Use Polynomial Regression (degree 2) to model 1YrReturn% based on SharpeRatio

Visualize with scatter plot and regression line

Observations

Highest 3-Year Return: Smallcap / Equity / High Risk fund (in sample dataset)

1-Year Return maximized at Sharpe Ratio: ≈ 1.8

PDF Export

Notebook exported to PDF using Jupyter nbconvert → PDF via LaTeX

If LaTeX is not installed, export as HTML → Print → Save as PDF

How to Run

Clone the repository:

git clone https://github.com/PROKILLER24/Python-Code.git
cd Python-Code


Activate virtual environment and install libraries

Open the notebook:

jupyter notebook Tradexa_Assignment.ipynb


Run cells top-to-bottom to reproduce analysis and plots

Notes

Dataset is synthetic for demonstration

All analysis, graphs, and insights are reproducible

README ensures easy understanding and replication of assignment
