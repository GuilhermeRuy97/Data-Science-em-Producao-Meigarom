# Feature Selection

> "A explicação mais simples sobre um fenômeno observado, deveria prevalecer sobre explicações mais complexas." (Occam's Razor)

Se você tem dois modelos que representa o mesmo fenômeno, dê preferência para o mais simples.

Ex:

![](https://i.imgur.com/KUE76vD.png)

# **Removemos Variáveis Colineares**

Ex,
Note que pneu e roda são colineares, assim como lanternas e faróis, parabrisa dianteiro e janela frontal

![](https://i.imgur.com/3sNAi9S.png)

------->

![](https://i.imgur.com/QmUgOsy.png)

**OS 3 MÉTODOS DE SELEÇÃO DE VARIÁVEIS**

**1. Seleção Univariada (Filter Methods)**<br>
-Classificar as variáveis como relevantes ou não

Relevância:<br>
Por exemplo, temos a porção venda que representa 100% do problema.
A variável Preço representar por exemplo, 20% do problema.
Anos representa 10%.
Promoção representa 50%.
Feriado representa 4%.<br>
Ou seja, promoção é a variável que mais explica o fenômeno e feriado a que menos explica (e poderia ser exclúido se fosse o caso).

Coeficientes de Correlação:
-Vai de -1 a 1, sendo o mais forte próximos de -1 e 1, e perto do 0 uma correlação fraca.<br>
Ex.<br>
Correlação forte<br>
![](https://i.imgur.com/Vk6Sgcd.png)<br>
Correlação fraca<br>
![](https://i.imgur.com/3nN4R1N.png)<br><br>
O que usar quandos as variáveis são de cada tipo?<br>
![](https://i.imgur.com/gAqiKlO.png)<br><br>
Vantagens e desvantagens da seleção univariada:
![](https://i.imgur.com/WLpeud3.png)




**2. Seleção por Importância (Embedded Methods)**<br>

Também conhecida como método embutido.
Em vez de utilizar a correlação como critério, utiliza-se a importância.
Usada em:
1. Random Forest <br>
Utiliza a Gini impurity:
Seleciona as variáveis e divide o conjunto de dados em outros dois conjuntos de dados, sendo estes dois novos conjuntos homogêneos entre si.
![](https://i.imgur.com/eG8yGpx.png)<br><br>
![](https://i.imgur.com/etL18gn.png)<br>

2. Lasso Regression<br><br>
![](https://i.imgur.com/E0rwVoG.png)
3. Ridge Regression


**3. Seleção por SubSet (Wrapper Methods)**<br>

 ![](https://i.imgur.com/Q7xPEHU.png)
Caso seja adicionado uma terceira variável e a performance não aumente, remove-se a variável.

O ALGORITMO BORUTA:
Faz-se uma cópia dos dados com as linhas embaralhadas para remover a correlação entre as variáveis.
Depois é encontrada a importância das features originais e das features embaralhadas.
Então, o algoritmo boruta compara a importância das variáveis originais com as da variável shadow (embaralhadas), se a originál for mais importante que a shadow, coloca-se 1 na tabela, caso seja menor, coloca-se 0. O nome dessa tabela é Success Counts.

![](https://i.imgur.com/PAYkhNe.png)

