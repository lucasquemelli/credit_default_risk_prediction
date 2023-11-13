# Credit Default Risk Prediction

<code><img width="100%" src="https://github.com/lucasquemelli/credit_default_risk_prediction/blob/main/Images/creditrisk.jpg"></code>

# 1. Business Problem

**Description**

To work with credit in the Finance Industry, firstly we must know: there are (1) a lender and (2) a borrower. The borrower repays the lender at a moment. At this scneario, there are two types of credit/loan: **(1) secured** and **(2) unsecured**. Secured loan is home loan, car loan or gold loan where the loan is secured by some assets (home, car or gold). Unsecured loans are those which are not secured by any assets, such as: personal loan, credit card, education loan or consumer loan.  

There are lending institutions or lenders that defines a rate of interest of loan. That defines the percentage of risk or percentage of loss they will take on the portfolio. The risks depend on the target lenders and on the type of loan. These are the major effects of the risks. 

Percentage of loss is (X amount of money not paid back)/(amount of money lended). Thus, the earning money is (1 - X)%. We may define people as n. Where ```n = (1 - X%)``` will pay back and ```n = X%``` will default. We can define the daulters as less to X, such as ```n < X%``` as well as the non defaulters (will pay back) such as ```n >= (1 - X%)```. We have to create a model to select these n percent of customers. 

From our population, we must classify our customers in 0 (not more than X%) or 1 (more than 1 - X%). **REMINDER:** The X% is defined by the business problem statement. To solve this problem, we created a Machine Learning algorithm to maintain the X% cutoff. 
