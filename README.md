# Titanic
Repositório criado para a **[competição do Kaggle sobre o desastre do Titanic](https://www.kaggle.com/competitions/titanic/overview)**

## [Etapa 1: Primeiro modelo](https://github.com/lucaslealx/Titanic/blob/main/Parte1.ipynb)
- Nesse etapa fizemos apenas o básico para conseguir verificar qual seria o resultado sem fazer nenhum tratamento nem engenharia dos dados
  - Foi visualizado um resumo da base utilizando o **[ydata-profiling](https://github.com/ydataai/ydata-profiling), biblioteca capaz de gerar com poucas linhas toda a descrição do nosso dataset**
  - Também **eliminamos colunas com elevada cardinalidade**, **tratamos valores vazios utilizando a média e a moda das variáveis** e **eliminamos todas as colunas de texto**
  - Criamos os modelos **utilizando 3 algoritmos: Árvore de Classificação, KNN e Regressão Logística** e **avaliamos esses modelos** utilizando a **acurácia** e a **matriz de confusão**
  - O score público retornado pelo Kaggle foi: 0,66746

