# Modelo de IA para Análise de Transição Energética

## Objetivo
Este projeto tem como objetivo analisar e prever dados relacionados à transição energética, com foco na produção e consumo de energia fotovoltaica. Foram desenvolvidos modelos de aprendizado de máquina para:
- Prever a produção de energia em uma região específica com base em variáveis climáticas e temporais.
- Identificar padrões de consumo e produção de energia, auxiliando na tomada de decisões para otimização de recursos e sustentabilidade.

Além disso, uma API foi criada utilizando Flask para disponibilizar os modelos preditivos em um ambiente web, permitindo integração prática.

---

## Descrição do Dataset
O dataset utilizado contém dados de 5 sistemas fotovoltaicos, registrados no arquivo `Inversors data`. Ele apresenta a produção diária de energia de sistemas solares. Após a limpeza e a organização, o dataset incluiu as seguintes colunas:

1. **Time**: Registro de tempo (não utilizado).
2. **Production (kW)**: Produção de energia fotovoltaica (variável alvo).
3. **Consumption (kW)**: Consumo energético (não relevante para este projeto).
4. **Temperature (℃)**: Temperatura registrada, influencia na produção.
5. **Weather**: Condições climáticas, categorizadas (ex.: Sunny, Cloudy).
6. **Date**: Data da medição.
7. **Hour**: Hora da medição.

Total de dados no Dataset: **25.493 Linhas** (incluindo os nomes das colunas).

---
### *[Link do dataset utilizado](https://www.kaggle.com/datasets/oakthyago/solarenergynor)*

---

## Estrutura do Projeto
### Etapas Desenvolvidas
1. **Coleta e Limpeza dos Dados**:
   - Dados organizados e preparados para análise.
   - Remoção de colunas irrelevantes (`Consumption (kW)` e `Time`).
   - Conversão de variáveis categóricas (ex.: `Weather`) para formato numérico.

2. **Modelos de Machine Learning**:
   - **Modelo 1: Previsão de Produção Energética**:
     - Algoritmo utilizado: Regressão Linear.
     - Objetivo: Prever a produção energética (`Production (kW)`).
   - **Modelo 2: Clusterização para Análise de Padrões**:
     - Algoritmo utilizado: K-Means.
     - Objetivo: Identificar padrões de produção com base em temperatura e clima.

3. **Visualizações**:
   - Gráficos para explorar e comunicar insights sobre a transição energética.
   - Exemplos: Comparação entre produção real e predita, padrões de clusters.

4. **Integração com Flask**:
   - API desenvolvida para disponibilizar os modelos preditivos em um ambiente web.
   - Suporte a endpoints para entrada de dados e retorno de previsões ou clusters.

---

## Requisitos do Projeto
### Instalação de Dependências
Instale as dependências do projeto utilizando o comando abaixo:
```bash
npm install
```

---

# Grupo EcoEnergy - 1TDSPW 

- Ruan Lima Silva - RM 558775
- Richardy Borges - RM 557883
- Henrique Izzi - RM 555413

---