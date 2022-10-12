# Implementation of different Value at Risk models (VaR models) for risk estimation


* **Normal Parametric Approach** assuming multi-variate normal distribution of daily returns. For this approach 
we need to calculate portfolio volatility which is done using different methods: 
  
  - *Equally weighted moving average*
  - *Exponential weighted moving average*
  - *Generalised Autoregressive Conditional Heteroscedasticity (GARCH(1,1)*
  - *Dynamic Conditional Correlation (Multivariate GARCH(1,1))*

*	**Non-parametric approach**: 

  * *Historical simulation* based on historical daily returns data
  * *Monte Carlo Simulation* of daily returns assuming normal distribution.

* **Parameters optimization** of GARCH(1,1) model and Multivariate GARCH(1,1) model with Maximum Likelihood Estimation.
  
*	Model validation with **back testing**, binomial confidence interval,  unconditional coverage test and independent test 

The *Var* folder contains the code for the implementation of the models described above. 
*model_comparison* folder includes  the analysis of the performance of the models for a 95% VaR for a portfolio of four 
stocks, finding that GARCH models overperforms the rest. *data_analysis* folder we analyse the normality of the
daily returns distribution
