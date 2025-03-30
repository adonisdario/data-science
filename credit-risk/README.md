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



Com o mapa de calor abaixo, podemos analisar melhor a distribuição das finalidades de empréstimos de cada classe:

heatmap

Um ponto extremamente importante da concessão de crédito é a manutenção de crédito, onde analisamos grupos que interessam e que não interessam, no intuito de mapear em quais grupos podemos aplicar diferentes estratégias de concessão e manutenção, como aumentar a concessão de crédito e os limites dos bons pagadores e grupos bem rankeados e bolar estratégias de recuperação, diminuição de limite ou até exclusão dos devedores da carteira de crédito. Por que focaríamos nossos esforços com indivíduos como João se 41.83% da nossa carteira de crédito possui casa própria ou tem emprego há mais de 10 anos? Indo além, ainda podemos criar uma nova classificação A+ para indivíduos que possuem ambas as características, ainda que seja um seleto grupo de 2.97%.

Estes bons grupos possuem altas rendas anuais. A média de renda do grupo A é de quase USD 95000, como João, mas diferente dele, o grupo A possui bons indicadores. Para se ter uma ideia, a probabilidade de um solicitante adimplente pedir um empréstimo, tal que não comprometa sua renda mensal em mais de 35%, é de 89.42%.

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



