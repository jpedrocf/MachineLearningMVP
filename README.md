# MachineLearningMVP

COMEÇAR UM DATASET NOVO COM INFOS QUE NÃO SEJAM DE REVENUE? CARACTERISTICAS DE ESTILO DE JOGO, GAMEPLAY, DESIGN...
Tentar localizar o reviewScoreClass com base nas outras métricas fornecidas, para checar quais métricas fazem um game ter bons reviews, colocar o que compõe o dataset, explicar que é uma reviewScoreClass é uma métrica criada, baseada na variável reviewScore


## Problem Definition
#### Objective:
The objective of this project is to develop a Machine Learning model capable of classifying a game's Review Score Class into three categories: Low, Medium, and High. This classification aims to identify and understand the key features that contribute to a game's evaluation.

## Problem Description
The problem involves analyzing game reviews (potentially sourced from gaming platforms, digital stores, or internal data). It is a multi-class classification problem, where the model is expected to categorize data based on a set of features provided in the dataset.

### Assumptions and Hypotheses:

#### Assumptions:

Features like copiesSold, price, revenue, avgPlaytime, and reviewScore have a direct or indirect relationship with the Review Score Class.
Data is consistent, meaning that the values for each metric (e.g., avgPlaytime or revenue) are accurately recorded and representative of the game's performance and reception.

#### Hypotheses:

Games with higher avgPlaytime and copiesSold are more likely to fall into the "High" category of the Review Score Class.
Games with lower price and higher revenue might attract more players, positively impacting their Review Score Class.
reviewScore serves as a strong indicator of the Review Score Class, showing clear thresholds for Low, Medium, and High.


## Constraints or Conditions for Data Selection
Only games with recorded reviews available in a structured format will be included.
The dataset must include at least three distinct classes for the Review Score Class: Low, Medium, and High.
The number of records (games) must be sufficiently large to train and evaluate the Machine Learning model, ensuring representativeness for each class.
The data must include at least some quantitative and qualitative variables that are interpretable in the context of game reviews.
Data containing missing values or anomalies will be treated or discarded to avoid negatively affecting the model.


## Dataset Description

For a detailed description of each attribute in the dataset, including definitions, data types, and value ranges, refer to the [Data Catalog](DataCatalog.md)
