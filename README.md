# Análise do Movimento dos Ventos — Dados Meteorológicos de Szeged (Hungria)

Este projeto realiza uma **análise exploratória e estatística dos ventos** na cidade de **Szeged, Hungria**, com base em dados climáticos coletados entre **2006 e 2016**.  
O estudo busca compreender padrões de velocidade e direção dos ventos ao longo do tempo, além de realizar classificações segundo a **Escala de Beaufort**.


## Objetivo

Explorar o comportamento dos ventos em diferentes **estações do ano, meses e horários**, identificando:
- Tendências de velocidade média do vento ao longo dos anos;
- Distribuições sazonais e horários de maior intensidade;
- Classificação dos ventos segundo a **Escala de Beaufort** (de calmaria a tempestade).


## Fonte dos Dados

- **Dataset:** [Szeged Weather Dataset (Kaggle)](https://www.kaggle.com/datasets/budincsevity/szeged-weather)
- **Período:** 2006 a 2016  
- **Localização:** Szeged, Hungria  
- **Origem:** Estações meteorológicas locais


## Etapas do Projeto

1. **Coleta e Leitura dos Dados**
   - Download automatizado do dataset via kagglehub.
   - Carregamento e visualização com pandas.

2. **Limpeza e Preparação**
   - Conversão da coluna de datas (Formatted Date) para o formato datetime.
   - Ordenação temporal e criação de novas colunas:
     - Ano, Mês, Dia, Hora e Trimestre.
   - Remoção de colunas redundantes (Loud Cover).

3. **Classificação de Velocidades**
   - Aplicação da **Escala de Beaufort**, categorizando velocidades em classes:
     - 0: Calmaria  
     - 1–3: Brisa leve  
     - 4–6: Vento moderado  
     - 7–12: Ventos fortes a tempestades  

4. **Análise Estatística e Visualização**
   - Cálculo de médias mensais, trimestrais e anuais.
   - Geração de gráficos de tendência temporal e distribuição.
   - Análise comparativa entre períodos sazonais.


## Tecnologias e Bibliotecas

- **Python 3**
- **Pandas** - Manipulação e limpeza de dados  
- **Matplotlib / Seaborn** - Visualizações e análise gráfica  
- **NumPy** - Operações numéricas  
- **KaggleHub** - Acesso automatizado a datasets do Kaggle  
- **Plotly** - Visualizações interativas
