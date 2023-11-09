# credit-rating-analysis

This code was developed to calculate an interest rate to charge a potential corporate borrower based on a simple risk-based pricing model.
The lending rate was calculated to take into account the borrower's credit risks (estimated from financial ratios), which was then used to estimate the Probability of Default (PD).
The final loan price was then calculated by adding PD- and Recovery Rate (RR)-based risk premia on top of the current risk-free rate.
Briefly, the steps of the calculations is as follows:

- Retrive fundamental accounting data for a listed construction company using yahooquery library
- Estimate credit rating based on Altman Z-score
- Based on the estimated credit rating, calculate PD using S&P's Average One-Year Transition Rates matrix
- Assign RR based on a current study, as well as estimate other parameters, & calculate final loan rate

The steps are also summarised in a diagram below. The code can be found in the [Jupyter notebook](https://github.com/R-Budhidarmo/credit-rating-analysis/blob/main/corporate_credit_risk.ipynb).

![Alt text](https://github.com/R-Budhidarmo/credit-rating-analysis/blob/main/corporate_credit_risk_workflow.png)
