# Modelos de MACHINE LEARNING

<br>

# Existem diversos tipos de algoritmos de Machine learning, como por exemplo:

__-Database mining:__
 Large datasets from growth of automation/web.<br>
 E.g., Web click data, medical records, biology, engineering.<br>
__-Applications can't program by hand:__
 Eg., Autonomous helicopter, handwriting recognition, most of Natural Language Processing (NLP), Computer Vision.<br>
__-Self-customizing programs:__
 E.g., Amazon, Netflix product recommendations.<br>
__-Understanding human learning (brain, real AI).__

# Mas o que é Machine Learning?

A definição mais comum que encontramos é a de um algoritmo que aprende realizar uma função sem ter sido especificamente programado para aquela função. Ou seja, dar ao computador a habilidade de aprender sem ter sido explicitamente programado para a tarefa.<br>
Dentro destes algoritmos, encontramos os __supervisionados__ e __não supervisionados__, além dos algoritmos de aprendizado por reforço, sistemas de recomendação etc.

# Supervised Learning

Chamamos de aprendizado de máquina supervisionado quando tentamos prever uma variável dependente a partir de uma lista de variáveis independentes. Como por exemplo:
![](https://i.imgur.com/cVcAXCL.png)
![](https://i.imgur.com/T1M951W.png)

Ou seja, o dados que utilizamos para treino __contém a resposta desejada__.<br>
Dentre as técnicas mais conhecidas para resolver problemas deste tipo, estão:<br>
-Regressão Linear;<br>
-Regressão Logística;<br>
-Redes neurais artificiais;<br>
-Máquina de suporte vetorial (Máquinas kernel);<br>
-Árvores de decisão;<br>
-K vizinhos mais próximos;<br>
-Bayes ingênuo; etc.

# Unsupervised Learning

Neste caso, o computador precisará descobrir perfis __sem dados anotados__ (sendo inclusive difícil de se avaliar este modelo não supervisionado). De uma forma geral, queremos achar uma representação mais informativa dos dados que temos. Temos como exemplo:
![](https://i.imgur.com/GttlPcV.png)
Dentre as técnicas mais conhecidas para resolver problemas deste tipo, estão:<br>
-Redes neurais artificiais;<br>
-Expectativa-Maximização;<br>
-Clusterização k-médias;<br>
-Máquinas de suporte vetorial (Máquinas Kernel);<br>
-Clusterização Hierárquica;<br>
-World2vec;<br>
-Análise de componentes principais;<br>
-Florestas isoladoras;<br>
-Mapas auto-organizados;<br>
-Máquinas de Boltzmann restritas;<br>
-Eclat;<br>
-Apriori;<br>
-t-SNE; etc.

![](https://i.imgur.com/iMSkx7i.png)


# Reinforced Learning

A aprendizagem por reforço consiste na maquina tentar aprender qual é a melhor ação a ser tomada, dependendo das circunstâncias na qual essa ação será executada. Ou seja, uma __recompensa ou punição__ é dada a um agente, dependendo da decisão tomada. Com o tempo, espera-se que o agente distingua quais ações geram recompensas e quais geram punições. <br>
Após conseguir ganhar a recompensa, o algoritmo pode tentar buscar por recompensas maiores através de uma __exploration__ ou, continuar com a recompensa segura sendo um __exploitation__.

![](https://i.imgur.com/1B8p4hg.png)


# Os 5 melhores modelos para se trabalhar (simples)

**1. Modelo de Média (average model)**
Serve como uma boa base comparativa pra performance dos outros modelos.
Por exemplo, um modelo com uma performance pior que a média, foi um modelo ruim.
**2. Linear Regression**
**3. Linear Regression Regularized (lasso)**
**4. Random Forest Regressor**
**5. XGBoost Regressor**
Usa a bagging e boosting