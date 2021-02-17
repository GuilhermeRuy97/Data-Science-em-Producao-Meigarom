
# **<center>CRISP-DS</center>**

**O QUE É?**<br><br>
-Um método de gerenciamento de projeto para Data Science;<br>
-CRISP = **CR**oss-**I**ndu**S**try **P**rocess - **D**ata **S**cience;<br>
-É um método cíclico de desenvolvimento.

**BENEFÍCIOS:**<br><br>
-A cada ciclo completo, temos uma uma versão End-to-End, ou seja, velocidade na entrega de valor.<br>
-Mapeamento de todos os possíveis problemas.

**ETAPAS:**<br><br>
**Questão de negócio:** Buscar o problema.<br>
**Entendimento do negócio:** Entender antes de começar a fazer. Muita vezes, quem te passou o problema pode não ter te passado a solução correta do problema, é necessário então, entender o real problema e analisar o que levou a pessoa a pensar naquela "solução anterior".<br>
**Coleta de Dados:** Uso de SQL e API's em tabelas para salvar os dados em um determinado ambiente.<br>
**Limpeza dos Dados:** Verificar caracteres especiais, tipos das strings, padronização entre os dados etc.<br>
**Exploração dos Dados:** Explorar por exemplo, quais fatores influenciam nas vendas (aumentar ou diminuir números de vendas).<br>
**Modelagem dos Dados:** Por exemplo, transformar variáveis categóricas em numéricas, transformar dados, variáveis respostas etc. Ou seja, preparar os dados para os modelos de machine learning.<br>
**Algoritmos de Machine Learning:** Aplicação dos algoritmos.<br>
**Avaliação do Algoritmo:** Criar um conjunto de erros que fazem sentido para o problema para verificar a acurácia, revocação, curva ROC, map, RMSE, tabela verdade etc, ou seja, métricas de erro.<br>
**Modelo em Produção:** Após o ciclo, caso o modelo possa, ele é colocado em produção.<br>
**Volta para o inicio** do ciclo em Entendimento do Negócio, por exemplo, adicionando Marketing ao negócio (ou outros fatores) para melhorar o restante do ciclo.


![](https://i.imgur.com/SzTh723.png)
<br>
<br>
**Ex. CRISP-DS no Desafio da Rossmann**<br>

> https://www.kaggle.com/c/rossmann-store-sales

**Questão de Negócio:**<br><br>
Qual é o valor das vendas de cada loja nas próximas 6 semanas?<br><br>
**Entendimento de negócio:**<br><br>
-Motivação: A previsão de vendas foi requisitada pelo CFO em uma reunião mensal sobre os resultados das lojas.<br><br>
-Qual a causa raiz do problema: Dificuldade em determinar o valor do investimento para Reformas de cada Loja.<br><br>
-Quem é o Dono do problema: Diretor Financeiro (CFO) da Rossmann.<br><br>
-Qual o formato da solução: Granularidade, Previsão de vendas por dia e por loja para os próximos 42 dias (6 semanas).<br><br>
-Tipo do Problema: Previsão de Vendas.<br><br>
-Potênciais Métodos: Séries temporais e Regressão.<br><br>
-Formato da entrega: 1) O valor total das vendas no final da sexta semana.<br> 2) Como estas vendas acontecem diariamente (podendo ser visto pelo celular).<br><br>
**Coleta dos Dados:**<br><br>
Disponível no Kaggle.<br><br>
**Update do Progresso do Projeto:**<br><br>
Mostrasse o que foi feito e descoberto até o momento do projeto, como os passos descritos acima. Isto pode gerar expectativa para as pessoas, pois saberão como esta o decorrer do trabalho, tranquilizando-as.<br><br>