# Quantitative Finance Bootcamp Projects (Summer 2025)

This repository contains a set of four mini projects completed as part of the **Quantitative Finance Summer Bootcamp** organized by the **Erdős Institute** in 2025. Each project applies foundational quantitative finance concepts using real-world data and Python-based analysis.

## Projects Overview

### Project 1: Portfolio Optimization

**Notebook:** `Mini_Project_1.ipynb`  

Constructed and analyzed **two investment portfolios** (high-risk and low-risk) using historical stock data (2015–2025) from Yahoo Finance.  
- Applied constraints on weight allocations
- Computed returns, volatilities, and Sharpe ratios
- Used `scipy.optimize` for portfolio weight optimization
- Visualized allocations and performance metrics

*Key Outcome:* Successfully optimized both portfolios under different risk constraints and quantitatively justified their profiles using Sharpe ratios and volatility-return tradeoffs.

---

### Project 2: Testing Normality of Returns

**Notebook:** `Mini_Project_2.ipynb`  

Tested the **normality assumption** in stock returns using:
- Shapiro-Wilk and D'Agostino-Pearson tests
- Rolling window normality testing
- Return filtering via clipping (to simulate outlier control)
- Comparison of raw vs. filtered return distributions

*Key Outcome:* Showed that while individual stocks often deviate from normality, filtered portfolios can exhibit closer-to-normal behavior. Visualized the evolution of p-values over time.

---

### Project 3: Option Sensitivities (Greeks)

**Notebook:** `Mini_Project_3.ipynb`  

Explored how **option price sensitivities** (Delta and Theta) vary with:
- Spot price (for a fixed time to maturity)
- Time to maturity (for a fixed spot price)

*Key Outcome:* Built intuition behind the Greeks and their dynamic behavior.

---

### Project 4: Delta and Sigma Hedging under Stochastic Volatility

**Notebook:** `Mini_Project_4.ipynb`  

Simulated stock paths using advanced volatility models:
- **Heston**, **SABR**, **GARCH(1,1)**, and a custom sigma model
- Implemented **Black-Scholes Delta Hedging**
- Extended to **Static and Dynamic Sigma (Vega) Hedging**
- Compared profit distributions across models

*Key Outcome:* Demonstrated the limitations of traditional delta hedging under non-constant volatility, and explored how vega exposure can improve hedging, especially for SABR-type dynamics.

---

## What I Learned
- How to apply statistical tests to financial return series
- Strengths and weaknesses of Black-Scholes assumptions
- Portfolio optimization under constraints
- Practical challenges of dynamic hedging strategies
- Importance of volatility modeling in risk management

---

### Repository Structure

<pre> <code> 
AB_Quant_Finance_Bootcamp_Summer25_Erdos/
│
├── Mini_Project_1.ipynb # Portfolio Optimization
├── Mini_Project_2.ipynb # Testing Normality of Returns
├── Mini_Project_3.ipynb # Option Sensitivities (Greeks)
├── Mini_Project_4.ipynb # Delta and Sigma Hedging under Stochastic Volatility
├── Test for Normality Notebook.ipynb # Supplementary analysis for normality testing
├── README.md
│
└── data/
├── high_risk_portfolio_weights.csv
├── low_risk_portfolio_weights.csv
├── prices.csv
└── log_returns.csv
 </code> </pre>

## Setup Instructions

 ### 1. Clone the Repository
 `https://github.com/AnweshaB12/AB_Quant_Finance_Bootcamp_Summer25_Erdos.git`

 ### 2. Create Environment with Requirements
 `conda env create -f environment.yml`

 ### 3. Activate the environment
`conda activate quant-finance-env`

## Usage

1. Launch the notebook interface:
`jupyter lab`

2. Open any of the four .ipynb notebooks.
You may edit or run them directly. Data is either downloaded using APIs (like yfinance) or provided in the data/ folder.
