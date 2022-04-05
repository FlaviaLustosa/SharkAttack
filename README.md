# SharkAttack

Primeiro Projeto IronHack

# Objetivo

O objetivo desse projeto é fazer a limpeza, dos dados de ataques de tubarões, com o intuito de saber se o ataque de tubarão é fatal e se existe algum mês que o ataque de tubarão é mais frequente!


# Extração dos dados

Os dados foram retirados do https://www.kaggle.com/datasets/teajay/global-shark-attacks .


# Limpeza dos dados

A tabela inicial tinha 25723 linhas em 24 colunas, mas a maioria dos dados eram nulos, como pode ver no gráfico abaixo:

<img style="-webkit-user-select: none;margin: auto;cursor: zoom-in;background-color: hsl(0, 0%, 90%);transition: background-color 300ms;" src="https://github.com/FlaviaLustosa/SharkAttack/blob/main/Grafico3.PNG" width="380" height="213">

Para realizar a limpeza, eliminei as colunas que praticamente não tinham dado. Utilizei o drop_duplicates para eliminas as linhas totalmente nulas ou repetidas e eliminei as linhas que não estavam pelo menos 50% preenchida.

Após limpeza restou 6302 linhas e 17 colunas deixando somente as colunas que iria utilizar na análise dos dados. 

A coluna Fatal estava preenchida de várias maneiras distintas foi necessário deixar apenas em 3 (Fatal, Não fatal e desconhecido) e a coluna de data além de escrita de várias maneiras distintas nem todas tinham informação de mês do ataque. Para limpar essa coluna criei uma coluna a parte com os meses de cada ataque para analisar melhor os dados.


# Conclusão

O risco de ataques de tubarão é relativamente baixo e se observa um aumento no número de casos no verão ou férias escolares, conforme pode ser visto no gráfico abaixo: 

<img style="-webkit-user-select: none;margin: auto;cursor: zoom-in;background-color: hsl(0, 0%, 90%);transition: background-color 300ms;" src="https://github.com/FlaviaLustosa/SharkAttack/blob/main/Grafico1.PNG" width="380" height="213">

O gráfico de ataques fatais por mês acompanha a curva de aumento de casos.

<img style="-webkit-user-select: none;margin: auto;cursor: zoom-in;background-color: hsl(0, 0%, 90%);transition: background-color 300ms;" src="https://github.com/FlaviaLustosa/SharkAttack/blob/main/Grafico2.PNG" width="380" height="213">
