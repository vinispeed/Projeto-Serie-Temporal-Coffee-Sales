# Análise de Séries Temporais - Vendas de Café

Este projeto tem como objetivo analisar e prever as vendas diárias de café em uma máquina de venda automática, utilizando técnicas de séries temporais. A análise é baseada em dados públicos disponíveis no [Kaggle](https://www.kaggle.com/datasets/ihelon/coffee-sales/data).

## Objetivos

- Explorar padrões de consumo, tendências e sazonalidades nas vendas de café.
- Aplicar modelos de previsão como Prophet e ARIMA.
- Comparar o desempenho dos modelos utilizando métricas quantitativas (MAE, RMSE) e validação cruzada temporal.
- Auxiliar na tomada de decisões estratégicas para o negócio, como reposição de estoque e promoções.

## Estrutura do Projeto

- **Importação e preparação dos dados:** Limpeza, tratamento de datas e agregação das vendas diárias.
- **Análise exploratória:** Visualização das vendas, médias móveis e identificação de datas faltantes.
- **Decomposição da série temporal:** Separação dos componentes de tendência, sazonalidade e ruído.
- **Modelagem:** Implementação dos modelos Prophet e ARIMA, com validação cruzada e previsão de 1 passo.
- **Comparação dos modelos:** Avaliação quantitativa e visual dos resultados.
- **Conclusão:** Discussão sobre o modelo mais adequado para a série analisada.

## Principais Resultados

- Ambos os modelos capturaram bem a tendência e a sazonalidade semanal das vendas.
- O modelo ARIMA apresentou desempenho quantitativo superior ao Prophet nas métricas avaliadas.
- Nenhum dos modelos conseguiu prever picos e vales extremos, comuns em séries com alta variabilidade.

## Como Executar

1. Certifique-se de que o arquivo index_1.csv está no mesmo diretório do notebook.
2. Abra o arquivo analise_serie_temporal_coffee_sales.ipynb em um ambiente como Jupyter Notebook ou JupyterLab.
3. Execute as células sequencialmente para reproduzir os resultados.

## Requisitos

- Python 3.8+
- pandas
- matplotlib
- seaborn
- statsmodels
- prophet
- scikit-learn
- numpy
- cmdstanpy

## Autor

- MArcos Vinicius da Silva

## Referências

- [Coffee Sales Dataset - Kaggle](https://www.kaggle.com/datasets/ihelon/coffee-sales/data)
- Documentação oficial do [Prophet](https://facebook.github.io/prophet/) e [ARIMA](https://www.statsmodels.org/stable/generated/statsmodels.tsa.arima.model.ARIMA.html)

---

Projeto desenvolvido para fins de estudo e demonstração de técnicas de séries temporais aplicadas ao contexto de vendas.