Group:

Adônis Dário: [Github](https://github.com/adonisdario)  | [LinkedIn](https://linkedin.com/in/adonisdario)

Caio Guedes: [Github](https://github.com/caiocguedes) | [LinkedIn](https://www.linkedin.com/in/caiocguedes)

Eveline Cavalcanti

Fernando Rangel

---

The analysis consists in applying statistic concepts in a Credit Concession of a bank. Through the data acquired by the bank, the group has to provide a report to the bank answering if the bank should or should not conced credit to a client.

The dataset used in this study can be found [here](https://www.kaggle.com/datasets/hetvigandhi03/loan-risk-analysis-dataset-real-world-data/data).

---

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

Analysing the group of default people, 36.8% of them applied for a loan to pay their credit card debt, which is a awful indicative. If a person needs to make a debt to pay another, what guarantees that the loan would be fulfilled?

With the heatmap below, we can discourse about the purpose of the loan for each rank class, along with the average annual income represented by the heat color.

![alt text](https://github.com/adonisdario/data-science/blob/main/credit-risk/images/heatmap.png?raw=true)

An important topic when conceding credit is credit maintenance, where it is discussed about what kind of loan and maintenance strategies is going to be applied for each rank, like raising credit concession and limits to good payers and create recovery strategies, lowering the limits or even excluding debtors from the credit portfolio. 
Therefore, why the bank should focus its attention to a client like John when 41.8% of the clients have their own house or have the same job for over 10 years, and John lacks both of these attributes?
OBS.: 2.9% of the clients have both an own house and work on the same job for over a decade. Therefore, these clients should be in a higher rank like A+.


Para deixar a situação de João ainda mais difícil, podemos analisar a distribuição da quantidade de contas adimplentes e inadimplentes da carteira de crédito utilizando a variável aleatória acc_now_delinq.

heatmap

Analisando com esta variável aleatória, fica evidente que não devemos conceder crédito para João.

Para fortalecer a nossa decisão, podemos ainda reforçá-la com os seguintes argumentos:

    Dentro da análise de crédito, no contexto da nossa carteira, torna-se interessante a concessão do mesmo mediante a condição de o solicitante ter, no máximo, 10 linhas de crédito já abertas (a depender da sua classificação no dataset, o valor pode ser menor). O propósito deste tipo de critério serve para mitigar o risco de inadimplência.

heatmap

Seguindo um raciocínio semelhante, mas analisando as contas INADIMPLENTES, a partir de um determinado número, a quantidade do valor do empréstimo é diminuída significativamente, reiterando a importância do prêmio de risco do crédito (que também pode ser justificado com o aumento na taxa de juros).

heatmap

Analisando o grupo E como um todo, podemos visualizar as distribuições amostrais de renda anual de acordo com o perfil do grupo. Em seguida, aumentaremos a quantidade de amostras para analisar o comportamento da distribuição à medida em que aumentamos, de maneira a observar a possível flutuação do salário de João, tornando mais previsível o comportamento de renda dele e possibilitando a tomada de decisão em relação à concessão de crédito.

heatmap

Como decisão final, optamos por não conceder crédito para João, tendo em vista que:

    Ele já está inadimplente
    Não possui renda comprovada
    Não tem garantias para pagamento de empréstimo
    Possui 35 linhas de crédito em aberto
    Está solicitando empréstimo para cobrir outras dívidas



