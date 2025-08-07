Criado por Adonis Dario | [LinkedIn](http://www.linkedin.com.br/in/adonisdario) | Email: dariopgm@gmail.com

Link para o notebook: [Ranking Brasil 2025](editar link)

Link para a planilha com o Ranking Completo [Ranking em Excel](editar link)

Link para a apresentação do LinkedIn: [Apresentação](https://www.canva.com/design/DAGkMUNMcpI/fQJ__UsIZh_A2C5tPTgFFw/edit?utm_content=DAGkMUNMcpI&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton)

# RANKING HISTÓRICO BRASIL 2025

Ranking dos maiores times do Brasil, que contabiliza as competições de âmbito nacional e internacional.

![alt text](https://github.com/adonisdario/data-science/blob/main/brasil-clubes-rank-2025/images/1.png?raw=true)

# Objetivo

O objetivo do estudo é construir um ranking histórico de todas as competições de Elite em que times brasileiros de futebol disputam.

1.	Primeiramente precisamos entender a pirâmide do futebol brasileiro e quais são as competições de Elite;
2.	Estabelecer métricas para a pontuação de cada competição e de cada posição conquistada por um time;
3.	Fazer um recorte dos 20 maiores clubes do Brasil, analisando a pontuação em cada competição e os troféus conquistados;
4.	Criar prateleiras com os times, ou seja, dividi-los em faixas de pontuação e observar a distância de pontos entre eles;
5.	Recorte dos maiores times do Norte-Nordeste e criar a faixa de pontuação;
6.	Processo de aquisição dos dados.

## AVISOS
1.	Para o Ranking de 2025 são retratadas as competições concluídas até 2024. Os títulos conquistados em 2025 serão contabilizados no ranking de 2026;
2.	O Ranking se limitará apenas ao desempenho esportivo obtido dentro de campo.
3.	Não serão contabilizados critérios subjetivos como influência no futebol brasileiro e internacional, movimentos humanitários feitos pelos clubes, etc.
4.	Também não serão contabilizados critérios como tamanho de torcida, engajamento em redes sociais, ou títulos em competições que este estudo não considera de "Competições de Elite".

# Atual Pirâmide do Futebol Brasileiro

![alt text](https://github.com/adonisdario/data-science/blob/main/brasil-clubes-rank-2025/images/4.png?raw=true)
	
  Atualmente, a base do Campeonato Nacional é o Campeonato Estadual. Um time que está apenas jogando o Estadual pode chegar ao topo em 5 anos via Campeonatos ou em 3 anos via Copas.
  
  Os campeonatos possuem um sistema de classificação e descenso para os melhores e piores times do campeonato, respectivamente. Já as Copas garantem a classificação para a Copa superior apenas se o time vencer o torneio. Tirando o Mundial, cada classificação garante um lugar no próximo ano.
	
  Para chegar ao topo da pirâmide, que é Torneio Mundial, via Campeonatos, um time que está apenas no Estadual, precisa terminar o Campeonato entre os melhores times do torneio que não estão nas divisões nacionais A, B ou C, para se classificar para a divisão D. Chegando na Série D, o time precisa ser um dos 4 melhores colocados de 8 do seu grupo na 1ª fase, passando para a fase eliminatória com 32 times. Os 4 times que chegarem na semifinal sobem para a Série C e disputam o título da D. Na Série C, o time precisa se classificar entre os primeiros 8 de 20 times da 1ª fase por pontos corridos e terminar entre os 2 melhores de 4 times do seu grupo da 2ª fase para subir para a Série B. Os primeiros colocados de cada grupo disputam o título da C. Na Série B, o time precisa se classificar entre os 4 primeiros do torneio de pontos corridos com 20 times para ascender à Série A. Na Série A, o time (geralmente) precisa terminar o torneio entre os 4 primeiros do torneio com 20 times para se classificar para a Copa Continental A (Libertadores). Chegando à Libertadores, o time precisa vencer o torneio com 32 times de quase todos os países da América do Sul para garantir a sua passagem para o Torneio Mundial no mesmo ano. No Torneio Mundial, o time precisa vencer o campeão da América do Norte, depois, o vencedor entre o campeão da África e Ásia para enfim enfrentar o campeão da Europa na grande final. Essa é a grande dificuldade de se tornar um campeão mundial e por isso vale a maior pontuação do ranking e o título de maior prestígio existente.

## Competições de Elite do Brasil
	
 Depois de conhecer a pirâmide do futebol brasileiro, chegamos nesta sub-pirâmide com as Competições de Elite. Essas são as competições que serão contabilizadas no ranking histórico.

![alt text](https://github.com/adonisdario/data-science/blob/main/brasil-clubes-rank-2025/images/5.png?raw=true)
 
  Percebemos que na base desta pirâmide estão a 1ª Divisão do Campeonato Brasileiro (Série A), a Copa do Brasil e a Copa Sulamericana. Todas estas competições garantem vaga à Copa Libertadores. Porém, atualmente, o Campeonato é jogado no formato de pontos corridos com 20 times. A Copa do Brasil é sempre no sistema eliminatório com cada time jogando contra 4 a 7 times. Já na Sulamericana, atualmente, joga-se contra 7 a 8 times, 3 numa fase de grupos e 4 em mata-mata.

1.	**Mundial de Clubes**: 15.000 pontos (100%)
2.	**Libertadores**: 6.750 pontos (45%)
3.	**Campeonato Brasileiro Série A**: 2.250 pontos (15%)
4.	**Copa do Brasil**: 2.100 pontos (14%)
5.	**Sulamericana**: 1.950 pontos (13%)

Comparando com a conquista Mundial, ganhar 3 Libertadores não seria equivalente, mas seria próximo em pontos. Lembrando que, para conquistar o Mundial é preciso conquistar a Libertadores.

Ganhar o Brasileiro 3 vezes é equiparado a ganhar 1 Libertadores, porém, ganhar a Copa do Brasil ou a Sulamericana 3 vezes chega próximo, mas não é equivalente. Colocamos uma grandeza de 3 vezes maior porque na Libertadores, os melhores times dos outros países da América do Sul também estão competindo pelo título e a vaga no Mundial.

O título das competições da base dessa pirâmide que traz mais prestígio seria o da 1ª Divisão, seguido da Copa do Brasil e da Sulamericana. Então por mais que elas estejam na mesma altura (garantam vaga para a Libertadores), há uma pequena diferença na pontuação de cada uma por causa do formato das competições e pelo valor subjetivo.

## Quanto vale não ser campeão?

* **Copas**:
1.	**Vice**: 33%
2.	**Semifinal**: 11%
3.	**Quartas**: 5%
4.	**Oitavas**: 3%
5.	**Fase de Grupos**: 1,5%
6.	**Fase Preliminar**: 0,3%

*	**Campeonato**:
1.	**Vice** : 33%
2.	**Top 4**: 23%
3.	**Top 8**: 17%
4.	**Top 12**: 12%
5.	**Top 16 / Não Rebaixado**: 8%
6.	**Top 24 / Rebaixado**: 5%
7.	**Top 32**: 4%
8.	**Top 64**: 2%
9.	**Top 100**: 1%

### Pontuações Exclusivas

*	**Mundial de Clubes**:
1.	**3º Lugar**: 16%
2.	**4º Lugar**: 11%

*	**Copa do Brasil**:
 _A nomenclatura abaixo se refere às fases anteriores às Oitavas de Final._
1.	**-1F**: 1,5%
2.	**-2F**: 0,7%
3.	**-3F**: 0,3%
4.	**-4F**: 0,1%

## Outras Competições de <ins>Elite</ins>

### Mundiais
	
 Existiram outras competições de Elite no passado. Umas foram equiparadas, unificadas ou reconhecidas como competições que chamamos de Elite.

 ![alt text](https://github.com/adonisdario/data-science/blob/main/brasil-clubes-rank-2025/images/9.png?raw=true)
 
*	**Taça Rio de 1951**: 6.000 pontos (40%)

A Taça Rio 1951 foi reconhecida como o 1º torneio mundial entre clubes. O objetivo era reunir campeões nacionais dos países da Europa que participaram da Copa do Mundo, para enfrentar os campeões do Campeonato Paulista (Palmeiras) e Carioca (Vasco da Gama), que eram os principais campeonatos estaduais da época, quando não existia campeonato Nacional no Brasil. Como esta competição foi criada antes da concepção das competições continentais e antes mesmo do Brasil ter um campeonato Nacional, não possui o mesmo prestígio que os outros títulos mundiais, e também está abaixo da Libertadores.

*	**Copa Intercontinental**: 12.750 pontos (85%)

A Copa Intercontinental foi o torneio criado em 1960 para definir o melhor entre o campeão da Libertadores (América do Sul) e o campeão da Champions League (Europa). Visto que o Intercontinental incluía apenas dois continentes, o Mundial da FIFA tem mais prestígio que a Copa Intercontinental.

*	**Mundial de Clubes de 2000**: 15.000 pontos (100%)

Como o Intercontinental não incluía os vencedores dos outros continentes, em 2000 a FIFA cria a 1ª edição do torneio mundial disputada por 7 equipes campeãs continentais, mais o Al-Nassr representando a Ásia, o Real Madrid como campeão da Champions de 1998 e o campeão de 1998 do país sede, Brasil, que foi o Corinthians. Como a competição foi disputada, em sua maioria, por campeões continentais, ainda que não fosse do ano ou da temporada anterior ao ano da competição, a competição é equiparável ao mundial de clubes como é atualmente.

### Campeonato Nacional

![alt text](https://github.com/adonisdario/data-science/blob/main/brasil-clubes-rank-2025/images/10.png?raw=true)

O Campeonato de 1937, o Torneio Roberto Gomes Pedrosa (Taça de Prata) e a Taça Brasil foram reconhecidos e equiparados como Campeonatos Brasileiros pela CBF (2.250 pontos).

### Copa Nacional B

A **Copa dos Campeões Regionais** foi uma competição que reunia, principalmente, os campeões dos campeonatos regionais, Copa do Nordeste, Copa Norte, Rio-São Paulo, Centro-Oeste e Sul-Minas. O vencedor deste torneio garantia vaga para a Libertadores do ano seguinte.
Conceitualmente, a Copa dos Campeões deveria ter mais prestígio que a Copa do Brasil. Porém, 3 dos 5 torneios regionais foram extintos, e com elas a Copa dos Campeões acabou, reduzindo a sua pontuação para ser equivalente a conquistar a vaga da Libertadores via Campeonato Nacional (1.050 pontos).

### Copa Continental B

![alt text](https://github.com/adonisdario/data-science/blob/main/brasil-clubes-rank-2025/images/11.png?raw=true)

A outra competição que deixou de existir foi a **Copa Conmebol**, a precursora da atual Sulamericana. Teve início em 1992 e foi extinta em 1999. Os times se classificavam via Campeonato Brasileiro. As primeiras colocações davam vaga para a libertadores, e as seguintes davam vaga à Copa Conmebol. Por terem os mesmos formatos de disputa e os mesmos critérios de classificação, a Copa Conmebol e a Sulamericana são equivalentes (1.950 pontos).

## COMPETIÇÕES BÔNUS

  Estas competições são consideradas bônus, pois são torneios que não escalam a pirâmide do futebol.

  ![alt text](https://github.com/adonisdario/data-science/blob/main/brasil-clubes-rank-2025/images/12.png?raw=true)

* Supercopas

A **Recopa Sulamericana** é a competição disputada, em dois jogos, entre os vencedores da Libertadores e da Sulamericana. Já a **Supercopa Rei** é o troféu disputado entre o campeão do Campeonato Brasileiro e o campeão da Copa do Brasil. Como a Recopa é um torneio internacional, tem um pouco mais de prestígio que a Supercopa Rei.

O cálculo da pontuação é feito a partir de 5% da média entre os títulos que cada equipe venceu. Ou seja, Recopa Sulamericana vale 217,50 pontos e a Supercopa Rei vale 109,50 pontos.

* Bônus Copa do Brasil

Entre 2001 e 2012 os times que participavam da Libertadores eram impedidos de competir na Copa do Brasil, e por isso, a CBF em seu ranking oficial concedia um bônus a esses times.

Para metrificar o bônus podemos nos basear que, de 2013 a 2020, quem participava da Libertadores entrava diretamente nas Oitavas de Final da Copa do Brasil, e de 2021 até o ano do ranking entra na 3ª Fase, por causa do aumento no número de times na competição, ou seja, 1 fase antes das Oitavas. Portanto, esse bônus será equivalente a ter chegado nas Oitavas de Final da Copa do Brasil (70 pontos).

# RANKING

## Por pontos:

![alt text](https://github.com/adonisdario/data-science/blob/main/brasil-clubes-rank-2025/images/15.png?raw=true)

O Estado de São Paulo é que mais tem times no Top 20 com 6, incluindo os 3 primeiros, São Paulo, Palmeiras e Santos. O 4º grande time do Estado, Corinthians, tem uma diferença de 18.5k de pontos e vê seus rivais a partir do 6º lugar do ranking. Guarani e Portuguesa são os últimos do Top 20.

O Rio de Janeiro também conta com seus 4 grandes times, mas o Flamengo (4º) possui uma diferença de pelo menos 49.4k de pontos sobre os seus rivais Vasco (10º), Fluminense (11º) e Botafogo (12º). Já a diferença média entre esses é de apenas 6.2k de pontos.

Estados com 2 times no Top 20 incluem o Rio Grande do Sul com Grêmio (5º) e Internacional (8º) tendo uma diferença de 20.4k de pontos entre eles; Minas Gerais com Cruzeiro (7º) e Atlético-MG (9º) separados por uma diferença de 19.5k de pontos; o Estado do Paraná contando com Athletico-PR (13º) e Coritiba (16º) tendo uma diferença de 12.9k de pontos e por fim o Estado da Bahia incluindo o Bahia (14º) e o Vitória (18º) separados por 6.1k de pontos.

Sport (15º) e Goiás (17º) são os representantes dos Estados de Pernambuco e Goiás no Top 20.

![alt text](https://github.com/adonisdario/data-science/blob/main/brasil-clubes-rank-2025/images/16.png?raw=true)

## Por troféus:

![alt text](https://github.com/adonisdario/data-science/blob/main/brasil-clubes-rank-2025/images/18.png?raw=true)

  Nota-se que o Palmeiras (23), Flamengo (21) e São Paulo (18) são os líderes em conquistas gerais. O São Paulo líder em Mundiais (3) e Continentais (7) e o Palmeiras lidera em conquistas Nacionais (18).
  
Apesar do Cruzeiro ter 5 troféus a mais que o Internacional, a diferença entre eles é de 3.2k de pontos. Isso mostra que o Inter mesmo sem ganhar títulos é sempre muito competitivo e faz boas campanhas. 

Guarani (19º) é o time de ranking mais baixo com um título. Já o Goiás (17º) é o time sem título com ranking mais alto.

![alt text](https://github.com/adonisdario/data-science/blob/main/brasil-clubes-rank-2025/images/20.png?raw=true)

## PORQUE O RANKING NÃO É POR TÍTULOS?

Porque o futebol não se resume a títulos e a grandeza desportiva de um time também está ligado às suas participações e campanhas nas Competições de Elite. Um exemplo prático é o Santo André e o Paulista, que apesar de terem conquistado a Copa do Brasil, o 1º time tem apenas 3 participações na Série A e o 2º não tem nenhuma. Assim, eles estariam na frente de times sem título como Goiás, Vitória, Fortaleza, Náutico, Ceará, Ponte Preta, Santa Cruz, e na frente de times que ganharam outros títulos continentais e nacionais como Chapecoense e Paysandu. Ninguém considera que Santo André e Paulista estejam no hall de maiores times do Brasil por causa deste título.

# ANÁLISE DE CASO

Goiás (17º), Vitória (18º) e Guarani (19º). Apenas Guarani possui um título, então porque ele está abaixo de Vitória e Goiás?

![alt text](https://github.com/adonisdario/data-science/blob/main/brasil-clubes-rank-2025/images/21.png?raw=true)

Pontuação por competições entre Goiás, Vitória e Guarani: 

![alt text](https://github.com/adonisdario/data-science/blob/main/brasil-clubes-rank-2025/images/22.png?raw=true)

Guarani está abaixo por causa do número de participações nas competições e também em boas campanhas na Sulamericana e Copa do Brasil. A baixa participação na Copa do Brasil se dá ao fato de que estando no Estado de São Paulo, onde tem 4 times grandes e outros times medianos, a disputa pela classificação na competição via Campeonato Estadual é mais acirrada que em outros Estados.

![alt text](https://github.com/adonisdario/data-science/blob/main/brasil-clubes-rank-2025/images/23.png?raw=true)

# PRATELEIRAS DO RANKING

Temos o Ranking, mas e se dividirmos os times em faixas de pontuação ou prateleiras, como ficaria? Para criar as prateleiras dos times foram testados os métodos de Sturges, Scott e Friedman-Diaconis. O objetivo é fazer uma análise do top 20 clubes do Brasil e estender um pouco o alcance, sem fazer uma análise de todos os times que já participaram de uma competição de Elite.

*	Friedman-Diaconis:
O método Friedman-Diaconis foi rejeitado por criar muitas faixas de pontuação com pouca diferença entre elas. Além disso, muitas faixas ficavam vazias pois a diferença entre a pontuação dos times varia muito. Com esse método, foram criadas 1394 prateleiras com apenas 62 preenchidas com times.

![alt text](https://github.com/adonisdario/data-science/blob/main/brasil-clubes-rank-2025/images/Regra_FD.png?raw=true)
![alt text](https://github.com/adonisdario/data-science/blob/main/brasil-clubes-rank-2025/images/Regra_FD_1.png?raw=true)
 
*	Sturges:
O método de Sturges também foi rejeitado pois ao contrário do Friedman-Diaconis este método criou apenas 10 prateleiras, com 1 vazia e a última prateleira aglutinada com 404 times. Para utilizar este método seria necessário criar sub-prateleiras com aquelas que possuem uma quantidade muito alta de times.

![alt text](https://github.com/adonisdario/data-science/blob/main/brasil-clubes-rank-2025/images/Sturges.png?raw=true)
![alt text](https://github.com/adonisdario/data-science/blob/main/brasil-clubes-rank-2025/images/Sturges_1.png?raw=true)
 
*	Scott:
O método de Scott é o intermediário entre Friedman-Diaconis e Sturges. Foram criadas 18 prateleiras de pontuação, mas com 12 prateleiras preenchidas e a última com 397 times aglutinados assim como no método de Sturges. Com muitas prateleiras contendo poucos times, outras vazias e outras com muitos times, este método foi rejeitado.

![alt text](https://github.com/adonisdario/data-science/blob/main/brasil-clubes-rank-2025/images/Scott.png?raw=true)
![alt text](https://github.com/adonisdario/data-science/blob/main/brasil-clubes-rank-2025/images/Scott_1.png?raw=true)

 
*	Cálculo pelo intervalo:
Pensando na análise de uma pequena parcela do total de times, foi definido o critério do cálculo pelo Intervalo da pontuação dos times, ou seja, a distância entre um time e seu antecessor. Levando em conta os 25 primeiros do ranking, podemos classificar as distâncias em 5 categorias variando de Muito Próximo a Muito Distante. Times com intervalos pequenos ficam juntos numa mesma prateleira. Quando a diferença for muito grande, uma nova prateleira é criada.

![alt text](https://github.com/adonisdario/data-science/blob/main/brasil-clubes-rank-2025/images/25.png?raw=true)
![alt text](https://github.com/adonisdario/data-science/blob/main/brasil-clubes-rank-2025/images/26.png?raw=true)
   
É notória a diferença de pontuação entre as prateleiras 5-6 (14.8k) e entre as prateleiras 6-7 (2.3k). Os títulos e a grande quantidade de participações nas competições de Elite estão concentrados nas 5 primeiras prateleiras. A 6ª prateleira é a última que tem times campeões do Campeonato Brasileiro. Abaixo dessa prateleira, tem alguns times que conquistaram a Copa do Brasil, mas que tem baixo número de participações e campanhas de destaque nas competições de Elite, por causa dos times das 5 primeiras prateleiras que ocupam as vagas dessas competições. Assim, os times da 6ª prateleira em diante tem menos chance de pontuar no ranking e a diferença entre eles seja próxima. Portanto, ao classificar uma distância como perto ou longe é preciso dar um peso para as prateleiras de 1-5 e outro peso para 6-10. Como é uma análise de um recorte, o critério manual foi escolhido, mas para uma análise completa seria necessário um dos critérios rejeitados acima.

## ANÁLISE DAS 5 PRIMEIRAS PRATELEIRAS

1.	São Paulo líder: 3 Mundiais, 3 Libertadores e 6 Brasileiros pesaram demais. Tem uma distância razoável para o vice líder Palmeiras;
2.	Tier 2 é formado por times vencedores de 3 Libertadores, com o Santos tendo 2 Mundiais, Grêmio e Flamengo com 1 e Palmeiras com a Copa Rio 51. Esses times têm uma média de 11 Títulos Nacionais e a distância média entre eles é próxima, apenas 3.8k de pontos;
3.	Tier 3 tem Cruzeiro e Internacional que venceram 2 Libertadores e o Corinthians 1. Já em títulos mundiais, Corinthians tem 2 e Internacional 1 Esses times tem uma média de 8 Títulos Nacionais. A distância média entre esses times é um pouco distante, 6.1k de pontos;
4.	Tier 4 possui Atlético-MG, Vasco e Fluminense vencedores de 1 Libertadores e uma média de 5 títulos Nacionais. A distância média entre os times é razoável, 4.9k de pontos;
5.	Tier 5 tem Botafogo e Athletico-PR; Libertadores: 1 título x 2 vices; Nacionais: 3x2; Sulamericanas: 1x2. A distância média é a maior entre as 5 prateleiras, 8.3k de pontos. O Bahia, que é o próximo do ranking, tem uma diferença para o Athetico-PR de 9.9k de pontos, mas como seu sucessor é o Sport com 3k de pontos, o Bahia cai para a 6ª prateleira.

![alt text](https://github.com/adonisdario/data-science/blob/main/brasil-clubes-rank-2025/images/27.png?raw=true)
 
A diferença média entre as prateleiras é de 22,3k. Mas em média, quantos pontos um time precisa para subir no ranking?

* 🟥 16.3k - Atlético-MG;
* 🟧 11.0k - Corinthians e Botafogo;
* 🟨 8.4k - Cruzeiro, Athletico-PR, Vasco e Palmeiras;
* 🟩 3.3k - Flamengo e Santos;
* 🟦 2.0k - Internacional, Grêmio, Fluminense

### Quem pode subir no ranking de 2026:

**Plausível**: Internacional, Grêmio e Fluminense subiriam com pelo menos 1 título nacional e uma boa campanha nas outras competições;
 	
**Difícil**: Flamengo teria que conquistar os dois títulos nacionais ou 1 título nacional e ser vice da Libertadores;

**Muito difícil**: Palmeiras teria que vencer obrigatoriamente a Libertadores e também 1 título nacional ou chegar pelo menos na semifinal do Mundial;

**Improvável**: Corinthians e Botafogo teriam que vencer obrigatoriamente a Libertadores, mas o Botafogo precisaria também de 1 título e 1 vice nacional e o Corinthians dos 2 títulos nacionais, completando a Tríplice Coroa inédita do Futebol Brasileiro;

**Impossível**: Atlético-MG, Cruzeiro, Athletico-PR, Vasco e Santos por não estarem na Libertadores de 2025, não têm chance de subir no ranking de 2026.

### Quem pode subir de prateleira no ranking de 2026:

Visto que os primeiros de cada prateleira são Palmeiras, Corinthians, Atlético-MG e Botafogo, e eles precisam de muitos pontos para subir no ranking, concluímos que, a não ser que um time tenha de 1 a 2 temporadas fantásticas com títulos grandes, não teremos um time subindo de prateleira nesse período. 

## ANÁLISE DAS PRATELEIRAS 6-10

![alt text](https://github.com/adonisdario/data-science/blob/main/brasil-clubes-rank-2025/images/31.png?raw=true)

A diferença média entre prateleiras 1-5 e 6-10 reduz de 22,3k para 1,4k. Por quê?

*	A prateleira 5 é a última a ter times com títulos continentais;
*	A prateleira 6 é a última a ter campeões da Série A:
o	Bahia com 2, Coritiba, Sport e Guarani com 1 título. OBS.: Sport venceu também a Copa do Brasil.
*	Apesar de Juventude¹ e Criciúma² terem vencido a Copa do Brasil e o Paysandu³ ter vencido a Copa dos Campeões, eles possuem poucas participações nas competições de Elite e, com isso, esses times fazem poucos pontos e não se distanciam dos outros times.
*	Nos Tiers 1-5 há 13 times que estão quase sempre na Série A. Sobra então 7 vagas para as prateleiras 6-10. Já na Copa do Brasil, que a classificação é via Campeonato Estadual, os times que estão em Estados mais "fortes" como São Paulo (São Caetano e RB Bragantino e Ponte Preta) têm dificuldades para classificar para esta competição e estarem aptos a pontuar.

![alt text](https://github.com/adonisdario/data-science/blob/main/brasil-clubes-rank-2025/images/32.png?raw=true)

Olhando a tabela percebe-se um declínio na média de participações nas competições de Elite à media que descemos as prateleiras, tirando assim a possibilidade de pontuação por parte dos times menores, e fazendo com que a diferença de pontos entre os times dos Tiers 1-5 seja maior do que os times dos Tiers 6-10.

Em média, quantos pontos um time precisa para subir no ranking?

* ⬛ 9,9k - Bahia;
* 🟥 2,8k - Sport e Portuguesa;
* 🟧 1,5k - Coritiba, Goiás, Vitória e Ponte Preta;
* 🟨 546 - Juventude, Santa Cruz e Paraná;
* 🟩 223 - Guarani e Fortaleza, Náutico, São Caetano e Paysandu;
* 🟦 32 - Criciúma, Bragantino e Ceará.

### Quem pode subir no ranking de 2026:

Em 2025, Bahia, Sport, Vitória, Fortaleza, Ceará, Juventude e Bragantino são os times participantes da Série A e Copa do Brasil, enquanto que Coritiba, Portuguesa, Náutico, Ponte Preta, Paysandu e Criciúma estarão apenas na Copa do Brasil. Considerando isso:

**Muito provável**: Ceará e Bragantino provavelmente subirão de posição no próximo ranking, mesmo se forem rebaixados;

**Plausível**: Criciúma precisa chegar na 3ª fase da Copa do Brasil;

**Difícil**: Para o Fortaleza, é preciso não ser rebaixado da Série A e chegar às Oitavas da Copa do Brasil, ou caso seja rebaixado, chegar às Quartas da Copa. Já o Paysandu precisa chegar nas Oitavas da Copa do Brasil;

**Muito difícil**: Náutico precisa chegar à Semifinal da Copa do Brasil. Juventude precisaria terminar no Top 4 da Série A e ser semifinalista da Copa do Brasil;

**Improvável**: Vitória precisaria de 1 título ou de vices na Copa do Brasil e Sulamericana e também assegurar o Top 4 da Série A. O Coritiba e a Ponte Preta precisam obrigatoriamente do título da Copa do Brasil. Sport precisa de 1 título e 1 vice nacional.

**Inimaginável**: O Bahia precisa obrigatoriamente do título da Libertadores e ou ser vice no Mundial ou 1 título e 1 vice nacional.

**Impossível**: Portuguesa por não estar na Série A e Goiás, Guarani, São Caetano, Santa Cruz e Paraná por não estarem aptos a pontuar, não tem possibilidades de subir no ranking.

*Percebemos que mesmo com diferenças de pontos pequenas, ainda é classificado como difícil um time dessas prateleiras subir no ranking. Por isso é necessário fazer um ajuste no recorte das prateleiras.*

# RANKING NORTE-NORDESTE

![alt text](https://github.com/adonisdario/data-science/blob/main/brasil-clubes-rank-2025/images/35.png?raw=true)

Percebe-se que os únicos representantes da região Norte são Paysandu e Remo, ambos do Estado do Pará. No Nordeste, confirma-se a percepção do G7 com Bahia e Sport no topo da pirâmide, Vitória isolado abaixo deles, Fortaleza e Náutico no 3º patamar, Ceará e Santa Cruz na base do G7.

1. Bahia e Sport: Únicos do Nordeste com títulos nacionais. Mesmo na mesma prateleira, Bahia tem 5.5k de pontos de vantagem juntando Série A, Libertadores e Sulamericana. O Sport leva vantagem nas Copas Nacionais com 2.5k pontos, totalizando uma vantagem de 3.1k de pontos pró Bahia;
2. Vitória isolado com 5k de pontos abaixo do Sport por causa da falta de títulos e 3k acima de Fortaleza e Náutico pelo alto número de participações na Série A e Copa do Brasil onde conquistou 1 vice em cada competição;
3. Fortaleza, Náutico e Ceará tem números semelhantes de vices e semifinais de Copa do Brasil, porém Fortaleza e Náutico têm maiores números de vices e Top4 da Série A. Fortaleza também leva vantagem em pontos na Sulamericana;
4. Paysandu e Santa Cruz tem pontos semelhantes na Copa do Brasil e Série A, mas o Paysandu leva vantagem por ter vencido a Copa dos Campeões Regionais e participado da Libertadores. A distância entre os times do Tier 3 e o Paysandu faz com que o Ceará esteja no Tier 4;
5. Remo e CSA são os times que menos participaram da Série A. O Remo leva vantagem na Copa do Brasil, participando de 32 edições e chegando em 1 semifinal, contra 21 participações do CSA com 1 quartas de final. Porém o CSA já foi vice da Copa Conmebol, fazendo com que a diferença entre eles seja de 248 pontos.

# PROCESSO DE AQUISIÇÃO DOS DADOS
	
  Todas as competições estão detalhadas ano por ano na wikipedia, com classificação final e chaveamento dos confrontos. Para cada competição foi construído um arquivo .ipynb para realizar o Web Scrapping de cada uma. O valor do título de cada competição fica em 100 pontos e segue as porcentagens anteriormente detalhadas para as outras posições.
  
  Construído o ranking da competição específica, foi gerado uma planilha .xlsx e armazenado no pasta [Tabelas](https://github.com/adonisdario/data-science/tree/main/brasil-clubes-rank-2025/tabelas) para serem acessados no arquivo principal. No arquivo principal essas planilhas são recuperadas e assim são dados os pontos para título definidos previamente. Como a porcentagem foi distribuída nos arquivos anteriores, ao aplicar a pontuação automaticamente sai a quantidade de pontos real de cada competição.
