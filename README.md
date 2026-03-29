# 📊 Projeto Cronos – Sistema Inteligente de Investimento com Machine Learning

O **Projeto Cronos** é um sistema completo de investimento quantitativo que integra **engenharia de features financeiras**, **clusterização avançada de ativos** e **redes neurais** para construção e avaliação de carteiras otimizadas no mercado brasileiro.

A proposta central é transformar dados históricos do mercado em **insights estruturados**, permitindo a seleção automatizada de ativos e a geração de portfólios com base em padrões estatísticos e aprendizado de máquina.

---

## 🚀 Principais Funcionalidades

* 📥 **Coleta de Dados Automatizada**
  Download de dados históricos de ações da B3 via Yahoo Finance.

* ⚙️ **Feature Engineering Otimizado**
  Cálculo de indicadores técnicos essenciais, como:

  * Retornos e volatilidade
  * RSI, MACD, ADX
  * Bandas de Bollinger
  * ATR e indicadores de volume

* 🔍 **Clusterização Híbrida de Ativos**
  Uso combinado de múltiplos algoritmos:

  * K-Means
  * Gaussian Mixture Models (GMM)
  * Spectral Clustering
  * DBSCAN

  O sistema seleciona automaticamente o melhor método com base no **Silhouette Score**.

* 🧠 **Rede Neural para Previsão de Retornos**
  Modelo baseado em TensorFlow (ou Random Forest como fallback) para prever retornos esperados dos ativos.

* 💰 **Geração de Carteira Otimizada (2024)**
  Alocação de pesos usando softmax sobre previsões do modelo.

* 📈 **Backtesting Completo**
  Avaliação da carteira comparada ao Ibovespa com métricas como:

  * Retorno total e anualizado
  * Volatilidade
  * Sharpe Ratio
  * Drawdown máximo
  * Alpha e Beta

---

## 🧩 Arquitetura do Sistema

O pipeline é dividido em quatro etapas principais:

1. **Clusterização (2017–2023)**
   Agrupamento de ativos com base em características técnicas.

2. **Treinamento da Rede Neural**
   Aprendizado com dados históricos (treino: 2017–2021, teste: 2022–2023).

3. **Geração da Carteira (2024)**
   Construção do portfólio com base nas previsões do modelo.

4. **Backtesting (2024)**
   Avaliação de desempenho frente ao benchmark (Ibovespa).

---

## 📁 Saídas do Sistema

O projeto gera automaticamente:

* `clusterizacao_resultados.json` → resultados dos clusters
* `carteira_2024.json` → composição da carteira
* `dados_tecnicos_otimizados.csv` → features calculadas
* `comparacao_desempenho_2024.png` → performance vs Ibovespa
* `drawdown_comparativo_2024.png` → análise de risco
* `retornos_mensais_2024.png` → retornos mensais

---

## 🎯 Objetivo

O Cronos busca responder à seguinte pergunta:

> *É possível construir uma carteira eficiente combinando clusterização de ativos e redes neurais?*

---

## ⚠️ Observações

* O sistema utiliza dados históricos e **não garante resultados futuros**.
* Parte das previsões de retorno é baseada em simulações estatísticas.
* Projeto com foco educacional e experimental em finanças quantitativas.

---


