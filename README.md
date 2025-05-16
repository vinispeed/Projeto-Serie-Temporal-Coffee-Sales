# Análise de Série Temporal: Vendas de Café

## Descrição

Este projeto realiza uma análise completa da série temporal das vendas diárias de café em uma máquina de venda automática. O objetivo é identificar padrões de consumo, tendências, sazonalidades e avaliar modelos de previsão para auxiliar na tomada de decisões estratégicas, como reposição de estoque e promoções.

## Base de Dados

- **Fonte:** [Kaggle - Coffee Sales Dataset](https://www.kaggle.com/datasets/ihelon/coffee-sales/data)
- **Arquivo:** `index_1.csv`

## Etapas do Projeto

1. **Importação de Bibliotecas**
2. **Carregamento e Visualização dos Dados**
3. **Análise Exploratória e Decomposição da Série**
4. **Teste de Estacionariedade (ADF)**
5. **Análise de ACF e PACF**
6. **Modelagem e Previsão**
   - Prophet
   - ARIMA
7. **Validação Cruzada Temporal**
8. **Comparação dos Modelos**
9. **Conclusão**

## Resultados

- Ambos os modelos (Prophet e ARIMA) capturaram bem a tendência geral da série, mas suavizaram as oscilações diárias.
- O ARIMA apresentou desempenho quantitativo ligeiramente superior ao Prophet nas métricas MAE e RMSE, tanto na previsão de 1 passo quanto na validação cruzada temporal.
- Nenhum dos modelos conseguiu prever picos e vales extremos, comuns em séries com alta variabilidade.

## Como Executar

1. Certifique-se de que o arquivo `index_1.csv` está no mesmo diretório do notebook.
2. Abra o arquivo `analise_serie_temporal_coffee_sales.ipynb` em um ambiente como Jupyter Notebook ou JupyterLab.
3. Execute as células sequencialmente para reproduzir os resultados.

## Requisitos

- Python 3.7 ou superior
- Bibliotecas utilizadas:
  - `pandas`
  - `numpy`
  - `matplotlib`
  - `seaborn`
  - `statsmodels`
  - `scikit-learn`
  - `prophet`
  - `cmdstanpy`

Instale as dependências com:
```
pip install pandas numpy matplotlib seaborn statsmodels scikit-learn prophet cmdstanpy
```

## Autor

Este projeto foi desenvolvido por Marcos Vinicius da Silva como parte de um estudo sobre previsão de séries temporais aplicadas a vendas.