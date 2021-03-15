# Exploração dos Dados

-Como modelar os dados para os algoritmos de machine learning.

"O aprendizado da maioria dos algoritmos de ML é facilitado com **dados numéricos** e na **mesma escala**"

<br>

**Como preparar os dados?**

**Normalização**:<br>
Reescala o centro para 0 com desvio-padrão igual 1.

**Rescaling**:<br>
-Reescala para o intervalo entre 0 e 1;<br>
-Distruições não Gaussianas (não possuem uma distribuição normal).

**Transformação**:<br>
-Conversão de Features Categóricas para Numéricas (Encoding);<br>
-Transformação de Natureza (exemplo, um ciclo de 1 ano  (de 1 a 12 meses)).

# **NORMALIZAÇÃO**

![](https://i.imgur.com/NRk0gOJ.png)
(valores - média) / desvio padrão

Após esse cálculo, temos uma coluna normalizada.

![](https://i.imgur.com/hdqy8xA.png)
 Após a normalização:
 ![](https://i.imgur.com/XmIUPPs.png)

*Nem todos os dados são bons para serem normalizados.

Exemplo de Rescaling para variáveis não normais.

**Min-Max Scaler**

Este algoritmo tende a não mudar a natureza das variáveis, mas sim, mudar o range delas. <Br>
*Este algoritmo é sensível a outliers.

![](https://i.imgur.com/XY1XW6T.png)
xmax - xmin = range

Após o min-max aplicado
![](https://i.imgur.com/cAht4iy.png)

<br><br>

**Robust Scaler**

Para evitar os problemas dos outliers, utiliza-se os quartis neste caso.

![](https://i.imgur.com/PcOlo3z.png)

Após o robust scaler
![](https://i.imgur.com/wVJQKj6.png)


# **FEATURES TRANSFORMATION - ENCODING**

Existem mais de 10 tipos de enconding para variáveis categóricas.
[https://towardsdatascience.com/all-about-categorical-variable-encoding-305f3361fd02]

Dica de **pacote**:
https://contrib.scikit-learn.org/category_encoders/

Tipos de Enconding (alguns deles)

**1.One Hot Encoding (ou dummy encoding)**

Beneficios: Fácil de aplicar<br>
Desvantagens: Cria muitas novas colunas no dataset<br>
Exemplos de uso: Feriados<br>
![](https://i.imgur.com/oNXTtIE.png)



**2.Label Encoding**<br>
Bom para variáveis com "nomes" sem uma relação entre sim, ex. nome de lojas
![](https://i.imgur.com/4qzR9C4.png)

**3.Ordinal Encoding**<br>
Parecida com o label, porém, há ordem.
![](https://i.imgur.com/2jbHR3z.png)

**4.Target Encoding**<br>
Bom quando há centenas de níveis em uma variável categóricas, por ex, cidades.<br>
Leva em consideração a variável.
![](https://i.imgur.com/9opaGUq.png)


**5.Frequency encoding**<br>
Faz uma contagem.
![](https://i.imgur.com/rZ89qE5.png)

**6.Embedding Encoding**<br>
Usado nas deep neural networks.
![](https://i.imgur.com/Ysa9Rd3.png)

**TRANSFORMAÇÃO DE NATUREZA**

**1.Logarithm Transformation**<br>
Transforma distribuições com skills muito à direita ou esquerda para mais próximas de uma normal.
![](https://i.imgur.com/NBDYn7g.png)


**2.Box-Cox Transformation**<br>
Utiliza uma fórmula.
![](https://i.imgur.com/dtSObPG.png)


**3.Cube-Root Transformation**<br>
Extrai a raíz cúbica dos valores.
![](https://i.imgur.com/DtmQXLP.png)


**4. Square-Roote Transformation**<br>
Extrai a raíz quadrada dos valores.

**5. Sine and Cosine Transformation**

<br>

![](https://i.imgur.com/PRmw9k7.png)
