# geofusion-case

Informações de negócio:
Uma empresa alimentícia situada no RJ deseja abrir filiais na cidade de São Paulo, tendo como público alvo adultos de 25 a 50 anos, das classes A (rendas A1 e A2) e B (rendas B1 e B2).

Ojetivo:
  A partir dos dados das lojas do RJ
  - estimar o faturamento que uma loja teria em cada um dos bairros;
  - classificar o potencial de cada bairro como Alto, Médio ou Baixo;
  - Segmentar os bairros de São Paulo de acordo com a renda e a idade, e indicar aqueles com maior aderência ao público alvo.

Informações técnicas:
A linguagem Python foi utilizada para realização da análise de dados e escolha do melhor modelo de regressão e de classificação.

Para estimar o faturamento das lojas de SP foram testas os modelos de regressão, Linear Regression, Support Vector Regression e Decision Tree Regressor. E utilizando Root Mean Squared Error para avaliação dos modelos. Com os resultados da base de treinamento e teste o modelo Decision Tree Regressor foi identificado como o melhor para o cenário. Em seguida foi utilizado o otimizador de hiperparâmetros chamado Random Search para tunar o modelo com o objetivo de alcançar uma resposta ainda mais precisa.

Para a classificação do potencial das lojas nos bairros de SP também foram testados três algoritmos, foram eles: Logistic Regression, k-Nearest Neighbors e Support Vector Machines. Lenvando a acurácia como métrica de classificação dos modelos, o modelo que obteve a melhor resposta foi o k-Nearest Neighbors.

Com os dados previstos de faturamento e de classificação para os bairros de SP gerei um Power BI para visualização dos resultados.
