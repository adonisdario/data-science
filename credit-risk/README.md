Group:

Adônis Dário: [Github](https://github.com/adonisdario)  | [LinkedIn](https://linkedin.com/in/adonisdario)

Caio Guedes: [Github](https://github.com/caiocguedes) | [LinkedIn](https://www.linkedin.com/in/caiocguedes)

Eveline Cavalcanti

Fernando Rangel

# Objetive

The analysis consists in applying statistic concepts in a Credit Concession of a bank. Through the data acquired by the bank, the group has to provide a report to the bank answering if the bank should or should not conced credit to a client.

The dataset used in this study can be found [here](https://www.kaggle.com/datasets/hetvigandhi03/loan-risk-analysis-dataset-real-world-data/data).

# Intro

Today the group will explore statistical concepts that could be applied on a real credit concession analysis. We will explore the case of John, who's applying for a loan to comply with his debts. The analysis will not only aplly to John but also to the group which he is.

Introducing John's case:

John is a young entrepreneur that is ranked on group E of the "bank" dataset. Borrowers within this low rank group have unattractive credit profile due to credit score, annual income, proof of income, lack of payments, between other factors that are important for a credit concession.

Why is John so low ranked?

* He is lacking payments (acc_now_delinq > 0);
* Although he claims to have an annual income of USD 95,000 this income hasn't been confirmed;
* He has 35 open credit lines. Meaning that if the client has this many open credit lines, he has finance problems;
* The purpose of the loan is to pay his credit card debt, which indicates a lack of finantial control;
* He pays rent
  > 39% of the borrowers also pay rent, which is factor to consider when conceding credit. The likelihood of default increases when the individual has rent to pay, as this is a guaranteed monthly deduction from their income.

# Discussion

Analysing the group of default people, 36.8% of them applied for a loan to pay their credit card debt, which is a awful indicative. If a person needs to make a debt to pay another, what guarantees that the loan would be fulfilled?

With the heatmap below, we can discourse about the purpose of the loan for each rank class, along with the average annual income represented by the heat color.

![alt text](https://github.com/adonisdario/data-science/blob/main/credit-risk/images/heatmap.png?raw=true)

An important topic when conceding credit is credit maintenance, where it is discussed about what kind of loan and maintenance strategies is going to be applied for each rank, like raising credit concession and limits to good payers and create recovery strategies, lowering the limits or even excluding debtors from the credit portfolio. 
Therefore, why the bank should focus its attention to a client like John when 41.8% of the clients have their own house or have the same job for over 10 years, and John lacks both of these attributes?

_OBS.: 2.9% of the clients have both an own house and work on the same job for over a decade. Therefore, these clients should be in a higher rank like A+._

Building a graph using the variable acc_now_delinq show us the percentage of clients that have open credit lines that are delinquent, which is almost 0,5%. Meaning that very few people is not fulfilling its payments and John is one of them.

![alt text](https://github.com/adonisdario/data-science/blob/main/credit-risk/images/inadprob.png?raw=true)

To reduce the risk of delinquency the criterion of the bank should consider 10 open lines of credit the ideal number and 20 the maximum for each. The graph shows that few people apply for more than 30 credit lines, meaning that these people has to be treated as exception and with extreme caution to avoid delinquency.

![alt text](https://github.com/adonisdario/data-science/blob/main/credit-risk/images/risco10contas.png?raw=true)

Back to delinquent accounts, the graph tells that from 1 delinquent account to 3 the average loan amount raises from USD 15,000 to USD 19,000 with USD 35,000 being the maximum amount that the bank had conceded. Having 4 or 5 delinquent accounts the average drops to USD 4,500 that justify the raise of the interest rate. John has 1 delinquent account of a loan amount of USD 25,000, half the amount of the maximum loan amount conceded by the bank.

![alt text](https://github.com/adonisdario/data-science/blob/main/credit-risk/images/contas_atraso_qtd_emp.png?raw=true)

Analysing rank E as a whole we can see the sampling distribution of annual incomes according to the groups’ profile. When raising the quantity of the sample, the distribution will change and with it John’s annual income floats making its behavior more predictable and helping the decision of conceding credit to him.

![alt text](https://github.com/adonisdario/data-science/blob/main/credit-risk/images/tlc.png?raw=true)

# Conclusion

In conclusion the report tells that John should not receive another credit line because:
*	He has a delinquent credit line
*	His annual income is not checked
*	He has no guarantees to pay its loans
*	Has 35 open credit lines
*	His loan purpose is to pay for other debts




