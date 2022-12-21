# Canhotos e as cobranças de penalty

## Introdução

Neste projeto rápido eu testo dois mitos frequentes sobre canhotos e cobranças de penalty. O primeiro mito é o de que "canhoto não sabe bater penalty". O segundo é o de que "canhoto perde penalty se bater no lado direito" (ponto de vista do batedor).

Eu testo esses dois mitos utilizando uma base com dados de todas as cobranças de penalty nas copas, entre 1982 e 2018. O conjunto de dados está disponível no link: https://www.kaggle.com/datasets/pablollanderos33/world-cup-penalty-shootouts?resource=download. 

## Análises preliminares

De forma geral, as porcentagens de acertos das cobranças à esquerda, centro e direita do gol são de 69.29%, 59.65% e 76.84%, respectively. Se olharmos para os canhotos apenas, esses números são respectivamente: 66.67%, 61.54% e 72.73%.

## Análise da diferença de acertos entre destros e canhotos

A porcentagem de successo dos destros nas cobranças é de 70.40% e dos canhotos é de 67.86%. Foi então testado se a diferença no sucesso nas cobranças é estatisticamente significante. Para tal, um teste do $\chi^2$ foi realizado.

As hipóteses nula e alternativa foram as seguintes:

$𝐻_0$ : A taxa de acerto de penaltis de canhotos e destros não apresenta diferença significativa.

$𝐻_1$ : A taxa de acerto de penaltis dos destros é maior dos que a dos canhotos.

Para realizar o teste do $\chi^2$, foi construí a matriz de contingência obtida dos dados e também a matriz esperada.

O valor de $\chi^2$ calculado na análise foi de $\chi^2_{\text{calc}} ~ 0.14$, que está abaixo do valor crítico para uma significância de 95%, $\chi^2_{\text{critico}} = 3.84.$

Também obteve-se o p-valor para esse teste que é igual a 0.71. 

Como o p-valor é maior que o nível de significância a hipótese nula não pode ser rejeitada. Portanto, não há diferença significativa entre destros e canhotos nos acertos de penaltis.

## Testando o mito de que canhotos erram penaltis cobrados à direita do gol

Neste caso, a hipótese foi a de que canhotos erram mais cobranças à direita do que à esquerda do gol.

Dessa forma, as hipóteses nula e alternativa foram formalizadas por:

$H_0$ : A taxa de acerto de penaltis dos canhotos das cobranças à direita e à esquerda do gol não apresenta diferença estatisticamente significativa.

$H_1$ : A taxa de acertos de penaltis cobrados por canhotos à esquerda do gol é maior do que a taxa de acertos à direita do gol.


