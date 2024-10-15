### Authors: [Adônis Dário](https://github.com/adonisdario), [Caio Guedes](https://github.com/caiocguedes), Eveline Cavalcanti e Fernando Rangel
# Cridit risk analysis using statistic methods

Let's explore how statistics concepts can be used to a real credit risk analysis.
Our study case will be a person named John, who is wanting a loan to fulfill his obligations.
Not only the analysis will apply to an individual, but also for the social group which he's in.

The dataset used can be found [here](https://www.kaggle.com/datasets/hetvigandhi03/loan-risk-analysis-dataset-real-world-data/discussion?sort=hotness).

## Introducing John's case

John is a young entrepreneur classified at group E, where low performance borrowers are ranked with a not attractive credit profile.
As we walk through John's information, we detect some interesting data for a rank E profile. So, why he's ranked so low?

1) He's a defaulter (**acc_now_delinq** > 0);
2) Although having a annual income of USD 95,000 his income could not be assured;
3) He has 35 open credit lines. Being a constant credit applicant means that he struggles finantially;
4) His loan objective is to pay a credit card debt, which is implies a lack of finantial control;
5) John pays rent.

Speaking of rent, 39% of the loan applicants currently pays rent, which is an alert to keep in mind when awarding credit to a phisics person. The probability of non-payment by a individual that pays rent increases because it is a constant expense on your income. Strike for John.

Looking deeply to the delinquent group, 36.8% of them applied for a loan to pay for the credit card debt. Applying for a loan to pay for a debt is a red flag. The applicant must have good warranties to get approved.

By the heatmap below we can analyse the distribution of the purpose of the loan for each rank. The collor tells the average annual income of each group and its purposes:

![heatmap](images/heatmap.png)

An extremely important matter of the credit concession is the credit maintenance, where we confirm which groups are interesting to conced credit loans, increase limits and which groups have to have recovery strategies, limit lowering or even exclusion of the credit lines. 
Why conced a credit line to John if 41.8% of the clients owns a house or are employed for at least 10 years? 
In fact, merging these two characteristics together we can create another rank A+ for 2.97% of the clients. These high ranked groups have a high annual income on average, like John's. However, unlike John people from high ranks have certified income. The probability of a client that's complient with its debts to apply for a loan that do not compromise its monthly income by 35%, is 89.4%.

To make thing even harder for John, by the chart below we see the probability of a client to have non complient lines of credit, using the **acc_now_delinq** column.

![heatmap](images/inadprob.png)

John have one non complient credit line, making him one of the 5% of the clients that have non complient credit lines. 
John should not have a new credit line.

Para fortalecer a nossa decisão, podemos ainda reforçá-la com os seguintes argumentos:

 - Dentro da análise de crédito, no contexto da nossa carteira, torna-se interessante a concessão do mesmo mediante a condição de o solicitante ter, no máximo, 10 linhas de crédito já abertas (a depender da sua classificação no dataset, o valor pode ser menor). O propósito deste tipo de critério serve para mitigar o risco de inadimplência.

 ![heatmap](images/risco10contas.png)

 Seguindo um raciocínio semelhante, mas analisando as contas INADIMPLENTES, a partir de um determinado número, a quantidade do valor do empréstimo é diminuída significativamente, reiterando a importância do prêmio de risco do crédito (que também pode ser justificado com o aumento na taxa de juros).

![heatmap](images/contas_atraso_qtd_emp.png)

Analisando o grupo E como um todo, podemos visualizar as distribuições amostrais de renda anual de acordo com o perfil do grupo. Em seguida, aumentaremos a quantidade de amostras para analisar o comportamento da distribuição à medida em que aumentamos, de maneira a observar a possível flutuação do salário de João, tornando mais previsível o comportamento de renda dele e possibilitando a tomada de decisão em relação à concessão de crédito.

![heatmap](images/tlc.png)

Como decisão final, optamos por não conceder crédito para João, tendo em vista que:

1) Ele já está inadimplente
2) Não possui renda comprovada
3) Não tem garantias para pagamento de empréstimo
4) Possui 35 linhas de crédito em aberto
5) Está solicitando empréstimo para cobrir outras dívidas

