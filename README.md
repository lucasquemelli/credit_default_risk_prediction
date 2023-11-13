# Credit Default Risk Prediction

<code><img width="100%" src="https://github.com/lucasquemelli/credit_default_risk_prediction/blob/main/Images/creditrisk.jpg"></code>

# 1. Business Problem

**Description**

---

To work with credit in the Finance Industry, firstly we must know: there are (1) a lender and (2) a borrower. The borrower repays the lender at a moment. At this scneario, there are two types of credit/loan: **(1) secured** and **(2) unsecured**. Secured loan is home loan, car loan or gold loan where the loan is secured by some assets (home, car or gold). Unsecured loans are those which are not secured by any assets, such as: personal loan, credit card, education loan or consumer loan.  

There are lending institutions or lenders that defines a rate of interest of loan. That defines the percentage of risk or percentage of loss they will take on the portfolio. The risks depend on the target lenders and on the type of loan. These are the major effects of the risks. 

Percentage of loss is (X amount of money not paid back)/(amount of money lended). Thus, the earning money is (1 - X)%. We may define people as n. Where ```n = (1 - X%)``` will pay back and ```n = X%``` will default. We can define the daulters as less to X, such as ```n < X%``` as well as the non defaulters (will pay back) such as ```n >= (1 - X%)```. We have to create a model to select these n percent of customers. 

From our population, we must classify our customers in 0 (not more than X%) or 1 (more than 1 - X%). **REMINDER:** The X% is defined by the business problem statement. To solve this problem, we created a Machine Learning algorithm to maintain the X% cutoff. 

The lender lends money to the borrower. The borrower pays back in 6 months (EMIs - equal monthly installments). This is our lending and its type is unsecured. 

DPD: days past due. This is the number of days by which moreover have missed an EMI payment. Let's assume a borrower needs to pay back by fifth of month M1: Bor = 5th day of M1. In case, borrower make a payment before fifth, the DPD will be zero because person has not breached the last payment date. In case the borrower pays after the fifth day, such as 7th, thus DPD will be the difference between these numbers: 7 - 5. The scenario where whoever has not made any payment post fifth of M1, then the snapshot date on which we are calculating DPD will be used: snapshot date - fifth date.  

The event when default is when a borrower goes to the **DPDx** (X) in payment of first **Yemi** (Y). **As DPD is in days**, therefore X can be 0, 10, 30, 60 or 90 days for example. **Y is the EMI**, therefore it is in number of installments, such as 1, 2, 3 or any number until 6. 

It is unlikely that customer will pay back the EMI after a DPD of 30 days, for example. They will achieve DPD 60, they will achieve DPD 90, and so on. Maybe, after 30 days a customer can pay back, but after 60 days is very unlikely. Thus 60 is going to be our threshold. To define the number of EMI payment after which a customer is unkely to pay back: if some person pays the first 3 EMIs, it is very unlikely they will default post that. Thus 3 will be our cutoff. 



