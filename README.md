# geofusion-case

Informações de negócio:
Uma empresa alimentícia situada no RJ deseja abrir filiais na cidade de São Paulo, tendo como público alvo adultos de 25 a 50 anos, das classes A (rendas A1 e A2) e B (rendas B1 e B2).

Objetivo:
  A partir dos dados das lojas do RJ
  - estimar o faturamento que uma loja teria em cada um dos bairros;
  - classificar o potencial de cada bairro como Alto, Médio ou Baixo;
  - Segmentar os bairros de São Paulo de acordo com a renda e a idade, e indicar aqueles com maior aderência ao público alvo.

Informações técnicas:
A linguagem Python foi utilizada para realização da análise de dados e escolha do melhor modelo de regressão e de classificação.

Para estimar o faturamento das lojas de SP foram testados os modelos de regressão, Linear Regression, Support Vector Regression e Decision Tree Regressor. E utilizando Root Mean Squared Error para avaliação dos modelos. Com os resultados da base de treinamento e teste o modelo Decision Tree Regressor foi identificado como o melhor para o cenário. Em seguida foi utilizado o otimizador de hiperparâmetros chamado Random Search para otimizar o modelo com o objetivo de alcançar uma resposta ainda mais precisa.

Para a classificação do potencial das lojas nos bairros de SP também foram testados três algoritmos, foram eles: Logistic Regression, k-Nearest Neighbors e Support Vector Machines. Lenvando a acurácia como métrica de classificação dos modelos, o modelo que obteve a melhor resposta foi o k-Nearest Neighbors.

Com os dados previstos de faturamento e de classificação para os bairros de SP gerei um Power BI para visualização e apresentação dos resultados.

Conclusão dos Resultados:
A partir das previsões estimadas pelos modelos pude concluir que SP é uma localidade com muito potencial a ser explorado. Apresentando quase 45% dos bairros estudados com potencial alto para abertura de uma loja. Outro dado interessante é o faturamento total previsto, superando os dados do RJ.
Focando no público alvo aderência a população de 25 a 34 anos e 35 a 49 anos foi de mais de 55%, ou seja, o somatório da população englobada nos bairros classificados como "Alto" foi de mais de 55% da população total.
Já a aderência para os domicílios de renda A1 e A2 superou os 70% e para B1 foi de 61,5% e B2 de 44,5%.

Próximos passos:
Alguns dados de renda média estavam faltando, e os tratei simplesmente tirando toda a informação daquela localidade. Um próximo estudo poderia atacar se há aumento nas métricas de avaliação dos modelos se algum método de preenchimento desse dados faltantes dosse implementado.
Outro ponto sensível é ação sobre os outliers. Como a base de dados era pequena resolvi manter os outliers mas também poderia ser outro ponto para possíveis verificações.
Outra forma para atacar esse problema em prol de ser mais ainda mais assertivo na estimação dos faturamentos, séria primeiramente classificar as regiões de SP e em seguida para cada nível gerar um modelo de regressão, ou seja, o nível Alto teria um modelo de regressão treinado somente com os dados dos bairros classificados como Alto.

Para agregar ainda mais ao banco de dados e provavelmente melhorar as previsões, dados como valor do ticket médio gastos em restaurantes do bairro, média do consumo de energia elétrica domiciliar e dimensões geográficas da localidade, seriam exemplos de dados que poderiam ajudar a alavancar o resultado.

