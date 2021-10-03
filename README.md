# AJUSTE DE CURVA POLINOMIAL COM PYTHON(Trabalh acadêmico)

## Descrição : Este trabalho destina-se ao conteúdo de Ajuste de Curvas Polinomial, sendo objeto de análise a Complexidade do Modelo e sua influência na Capacidade de Generalização (observação de dados novos). Os passos para execução do trabalho são os seguintes:

## O trabalho foi baseado no livro "Neural Networks for Pattern Recognition" de Christopher M. Bishop

1) Utilizar a função geradora h(x)=-0.85*exp(0.90*x) + 0.36 + 0.12*sen(5*pi*x)
2) Gerar inicialmente um conjunto de dados, atribuindo valores a x (sugestão: x=(0.0:0.05:1.0),
com N exemplares, neste caso 21 exemplares.
3) Separar os dados gerados em dois conjuntos: Treinamento (2/3 dos exemplares – xtr e htr) e
Teste (1/3 dos exemplares – xte e hte).
4) A cada ponto de dado (valor de x) do Conjunto de Treinamento (xtr) ser acrescentado um
ruído gaussiano com média zero e desvio padrão igual a 0,05, obtendo um novo Conjunto de
Treinamento xtrp.
5) Para obtenção dos parâmetros livres W* (parâmetros ótimos), através do conjunto de
treinamento, deve ser utilizada a função POLYFIT(xtrp,htr,M), onde M é a ordem do
polinômio, obtendo-se y(xtrp)= w1x
m + w2x
m-1 +...+ wmx + wm+1. A função POLYFIT retorna um
vetor com os parâmetros dos livres do polinômio (ex.: m=1, vetor W*<w1 w0>, m=3, W*<w4 w3
w2 w1 w0>).
6) Fazer simulações para m=1, m=3, m=5, m=7, m=9 e m=11 e superior, se necessário.
7) Uma vez obtido W* para cada ordem, plotar, para cada ordem, a curva htr/y(xtrp) (curva
ajustada para os dados de treinamento). Use a função POLYVAL para testar o polinômio
obtido. Para efeito de análise deve ser também plotado hte/y(xte)’ (curva da função ajustada
do conjunto de teste).
8) Computar os E^RMS (root-mean-square error) para o conjunto de treinamento e para o conjunto
de teste. Vale ressaltar que htr e hte são os valores desejados e y(xtrp) e y(xte) são os
valores calculados. Comparar, para cada grau de polinômio simulado, o erro em função dos
graus do polinômio (curva ERMS x grau do polinômio).
9) Fazer as análises necessárias quanto a relação da complexidade do modelo pela capacidade
de generalização. Escolher o melhor grau do polinômio que ajusta os dados. Utilizar o Cap. 1,
item 1.5 do livro "Neural Networks for Pattern Recognition", Christopher M. Bishop, como
referência para o trabalho.
10) Repetir a operação(itens 2 ao 9) para N = 200 exemplares
11)Utilizar a Regularização para a melhor equação ajustada (melhor valor de M) para este
conjunto com 200 exemplares. Utilize 3 valores de lambda (slides).
12) Apresentar o trabalho escrito com os resultados no formato paper (duas colunas)
