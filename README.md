## Previsão de Temperatura com SARIMAX

Este repositório contém o código para previsão de temperatura usando o modelo SARIMAX. O modelo é treinado em dados históricos de temperatura e utilizado para gerar previsões de temperatura futura.

### Descrição

O código implementa as seguintes etapas:

1. **Carregamento dos dados:** O código carrega dados históricos de temperatura a partir de um arquivo Excel.
2. **Pré-processamento dos dados:** Os dados são convertidos para uma série temporal, com a data como índice.
3. **Análise exploratória de dados:** A série temporal é analisada para identificar padrões, como tendências e sazonalidade, usando gráficos de linha, decomposição da série temporal e autocorrelação.
4. **Seleção do modelo:** O código usa a função `auto_arima` para determinar os parâmetros ideais para o modelo SARIMAX, otimizando para minimizar o erro quadrático médio (RMSE).
5. **Treinamento do modelo:** O modelo SARIMAX é treinado usando os dados históricos.
6. **Previsão:** O modelo treinado é usado para gerar previsões de temperatura para os próximos 90 dias.
7. **Avaliação:** As previsões são avaliadas usando o RMSE.
8. **Visualização:** Os resultados são visualizados em gráficos, mostrando as previsões, dados históricos, intervalo de confiança e RMSE.

### Como usar

1. Clone este repositório.
2. Substitua o arquivo "temperature.xlsx" com seus próprios dados de temperatura.
3. Execute o notebook Jupyter ou o script Python.

### Dependências

- pandas
- matplotlib
- statsmodels
- pmdarima

### Resultados

O código produz previsões de temperatura para os próximos 90 dias, junto com um intervalo de confiança. O RMSE é usado para avaliar a precisão das previsões.

### Notas

- O modelo SARIMAX é uma ferramenta poderosa para previsão de séries temporais, mas requer dados históricos de alta qualidade para alcançar resultados precisos.
- Os parâmetros do modelo podem ser ajustados para otimizar a precisão das previsões.
- O código pode ser modificado para usar outros conjuntos de dados de temperatura ou para gerar previsões para períodos de tempo diferentes.
