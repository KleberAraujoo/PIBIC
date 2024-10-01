# PIBIC - Programa Institucional de Bolsas de Iniciação Científica

<h1>Métodos de Agrupamento Difuso Multivariado usando Distância de City Block</h1>

<h4>Aluno: Kleberson de Araújo Bezerra 
<h5>Lattes: http://lattes.cnpq.br/4354434691905652</h5>
<h4>Orientadora: Profa. Dra Renata Maria Cardoso Rodrigues</h4> 
<h5>Lattes: http://lattes.cnpq.br/9289080285504453</h5>

<h3>Introdução e Justificativa</h3>
  Este projeto de pesquisa tem como objetivo avançar o estado da arte das técnicas de agrupamento do tipo partitivo, por meio do desenvolvimento de pesquisa básica sobre métodos de agrupamento no paradigma difuso, com base em vetores de medianas e graus de pertinência multivariados. Serão consideradas distâncias ponderadas e não ponderadas para refinar o processo de agrupamento. Além disso, será realizada uma avaliação experimental com dados sintéticos e reais. Os métodos propostos serão comparados com técnicas tradicionais de agrupamento difuso baseadas em medianas, que não levam em conta os graus de pertinência multivariados na presença de dados aberrantes.

<h3>Objetivos</h3>
  Este trabalho propõe um método de agrupamento difuso utilizando a distância City Block (norma L1), onde os graus de pertinência de cada objeto a um determinado grupo são representados por um vetor p-dimensional, onde p é o número de variáveis. Isso permite calcular a similaridade de um objeto em relação a um protótipo com base em cada variável. A proposta é fornecer uma maior quantidade de informações para o algoritmo difuso, visando melhorar a qualidade dos agrupamentos em comparação com métodos tradicionais que não utilizam graus de pertinência multivariados. O estudo busca responder a duas principais perguntas de pesquisa: (1) É possível melhorar a qualidade dos agrupamentos difusos utilizando a distância City Block em conjunto com graus de pertinência calculados para cada variável? (2) É possível descrever a relevância de cada variável para cada grupo utilizando esses graus?

<h3>Metodologia</h3>
  Os métodos de agrupamento do tipo partitivo geram uma única partição dos dados, em vez de uma série de partições encadeadas. A determinação do número de grupos desejados pode ser desafiadora, especialmente na ausência de informações prévias suficientes sobre o conjunto de dados. Métodos particionais se dividem em duas principais categorias: rígidos e difusos. Nos métodos rígidos, os objetos pertencem a exatamente um grupo, com grau de pertinência no conjunto {0, 1}, sendo 1 quando o objeto pertence ao grupo e 0 caso contrário. O método mais popular dessa categoria é o K-Means. Já nos métodos difusos, os objetos possuem graus de pertinência para todos os grupos, variando no intervalo [0,1]. O método difuso baseado na distância City Block, amplamente utilizado na literatura, tem a vantagem de ser menos sensível a outliers ou ruídos. No entanto, não oferece uma forma de analisar quais variáveis foram mais importantes para definir o grau de pertinência final.

  Neste projeto, propomos calcular o grau de pertinência multivariado para cada objeto em relação a cada variável individualmente, o que traz duas vantagens: (1) a possibilidade de interpretar a pertinência de um objeto a um grupo em função de cada variável e (2) a obtenção de mais informações dos dados, resultando em uma maior qualidade de agrupamento. As etapas do estudo incluem: (1) Implementação de um ambiente experimental para avaliar a abordagem proposta com dados artificiais, (2) Avaliação do desempenho dos métodos utilizando o índice corrigido de Rand (medida da proximidade entre uma partição a priori e a obtida pelo método) e a taxa de erro de classificação, (3) Validação com dados reais, utilizando conjuntos de dados intervalares de repositórios de Machine Learning e outros conjuntos relevantes. As medidas serão estimadas pelo método Monte Carlo, com 100 replicações para cada conjunto. Finalmente, será realizado um estudo comparativo entre o método proposto e o método tradicional de agrupamento baseado na distância City Block que não utiliza graus de pertinência multivariados. Os métodos serão implementados em Python.

<h3>Habilidades Adquiridas</h3>
Desenvolvimento de algoritmos de agrupamento no contexto da inteligência computacional.

<h3>Referências</h3>
[1] Bezdek, J. C. (1981). Pattern Recognition with Fuzzy Objective Function Algorithms. Plenum Press, New York. [2] Pimentel, B.A. e Souza, R.M.C.R. (2013). A Multivariate Fuzzy C-Means Method. Applied Soft Computing (Print). Applied Soft Computing, v.13, p.1592 - 1607. [3] Jajuga, Krzysztof (1991) L1-norm based fuzzy clustering. Fuzzy Sets and Systems 39 (1991) 43-50. [4] Jain, A. K., Murty, M. N., & Flynn, P. J. (1999). Data clustering: a review. ACM computing surveys (CSUR), 31(3), 264-323. [5] Jain, A. K. (2010). Data clustering: 50 years beyond K-means. Pattern Recognition Letters, 31(8), 651-666.



