# Projeto: Simulação de Classificação de Carros Usando Árvores de Decisão

Este projeto de machine learning simula a classificação de carros com base em dados como preço, idade do modelo e quilômetros rodados por ano. O objetivo é treinar um modelo capaz de prever se um carro foi vendido ou não, utilizando técnicas de validação cruzada (`GroupKFold`) e exploração de hiperparâmetros em árvores de decisão.

## Descrição do Projeto

Neste projeto, utilizamos diversos algoritmos e técnicas de machine learning para simular o agrupamento e classificação de dados de carros, em especial o `DecisionTreeClassifier` da biblioteca `sklearn`. Além disso, foi explorado como o modelo se comporta ao ser treinado e testado com diferentes grupos de dados (agrupados por modelo de carro) e diferentes hiperparâmetros.

## Estrutura do Projeto

1. **Importação e Tratamento de Dados**
   - Dados importados a partir de um repositório externo.
   - Remoção de colunas irrelevantes e ordenação de dados conforme necessidade.

2. **Modelos de Classificação**
   - Utilização de `DummyClassifier` para estabelecer uma baseline.
   - Implementação de `DecisionTreeClassifier` para a criação de modelos mais robustos.

3. **Validação Cruzada com `GroupKFold`**
   - Aplicação de validação cruzada usando `GroupKFold` para testar a performance do modelo ao separar grupos com base no modelo do carro.

4. **Exploração de Hiperparâmetros**
   - Realização de testes variando os parâmetros `max_depth` e `min_samples_leaf` da árvore de decisão.
   - Avaliação do desempenho dos modelos com diferentes combinações de parâmetros para evitar overfitting e underfitting.

5. **Visualização e Análise de Resultados**
   - Gráficos de linhas, heatmaps e pairplots para analisar correlações entre os parâmetros e o desempenho do modelo.
   - Análise de overfitting e identificação do melhor conjunto de parâmetros.

## Tecnologias Utilizadas

- **Python 3.8+**
- **Bibliotecas:**
  - `pandas`
  - `numpy`
  - `scikit-learn`
  - `seaborn`
  - `matplotlib`
  - `graphviz`

## Como Executar o Projeto

1. **Instalar dependências:**
   Execute os seguintes comandos para instalar as bibliotecas necessárias:

   ```bash
   !pip install graphviz==0.9
   !pip install pydot
   !pip install seaborn==0.9.0
   !apt-get install graphviz
   ```

2. **Carregar e preparar os dados:**
   Os dados são carregados diretamente de uma URL e preparados para serem usados no modelo.

3. **Treinar e avaliar o modelo:**
   Utilize o código para rodar a validação cruzada e visualizar os resultados com diferentes hiperparâmetros.

## Resultados

- O projeto explora o impacto de diferentes profundidades de árvore e tamanhos mínimos de amostras em folhas, buscando o melhor equilíbrio entre o desempenho em dados de treino e teste.
- Um dos principais objetivos é minimizar o overfitting, ajustando o modelo para que ele tenha um bom desempenho em dados novos (não vistos).

## Exemplos de Visualizações

- **Gráfico de Desempenho (Treino x Teste):**
  ![Gráfico de Desempenho](link_para_o_grafico.png)

- **Heatmap de Correlações:**
  ![Heatmap de Correlações](link_para_o_heatmap.png)

## Conclusão

Este projeto é um ótimo exemplo de como a validação cruzada pode ser usada para testar o desempenho de um modelo com diferentes grupos de dados e como a exploração de hiperparâmetros pode otimizar o desempenho de um modelo de árvore de decisão.
