# Titanic
Repositório criado para a **[competição do Kaggle sobre o desastre do Titanic](https://www.kaggle.com/competitions/titanic/overview)**

## [Etapa 1: Primeiro modelo](https://github.com/lucaslealx/Titanic/blob/main/Parte1.ipynb)
- Nesse etapa fizemos apenas o básico para conseguir verificar qual seria o resultado sem fazer nenhum tratamento nem engenharia dos dados
  - Foi visualizado um resumo da base utilizando o **[ydata-profiling](https://github.com/ydataai/ydata-profiling), biblioteca capaz de gerar com poucas linhas toda a descrição do nosso dataset**
  - Também **eliminamos colunas com elevada cardinalidade**, **tratamos valores vazios utilizando a média e a moda das variáveis** e **eliminamos todas as colunas de texto**
  - Criamos os modelos **utilizando 3 algoritmos: Árvore de Classificação, KNN e Regressão Logística** e **avaliamos esses modelos** utilizando a **acurácia** e a **matriz de confusão**
- O **score público retornado pelo Kaggle foi: 0,66746**

## [Etapa 2: Tratando as variáveis de texto](https://github.com/lucaslealx/Titanic/blob/main/Parte2.ipynb)
- Na segunda etapa o foco principal foi tratar as variáveis de texto para conseguirmos utilizar todas as variáveis no nosso modelo
  - Se quiser **saber mais sobre tratamento de variáveis de texto**, você pode **conferir [esse artigo que eu escrevi no Medium](https://medium.com/@llucaslleall/tratando-vari%C3%A1veis-categ%C3%B3ricas-em-projetos-de-ci%C3%AAncia-de-dados-834dcc5bb636)**
  - Para fazer esse tratamento, utilizamos **lambda function e OneHotEncoder**
- Utilizamos os mesmos modelos vistos anteriormente
- O **score público retornado pelo Kaggle foi: 0,76555**

## [Etapa 3: Entendendo mais profundamente o negócio e melhorando os tratamentos dos dados](https://github.com/lucaslealx/Titanic/blob/main/Parte3.ipynb)
- Na terceira etapa o grande objetivo era **entender melhor os dados** para **fazer um melhor tratamento** e tentar melhorar o resultado obtido anteriormente.
- Então fizemos:
  - O **ajuste na escala dos dados para as colunas Age e Fare**
  - Entendemos melhor as colunas **SibSp** (nº de irmãos/cônjuges a bordo do Titanic) e **Parch** (nº de pais/filhos a bordo do Titanic) e criamos **2 novas colunas: total de familiares a bordo do navio e se o passageiro estava sozinho ou não**
  - Para finalizar, analisamos a **correlação de todas as variáveis** para selecionar aquelas que mais faziam sentido para o modelo
- Utilizamos os mesmos modelos vistos anteriormente
- O **score público retornado pelo Kaggle foi: 0,76555**
