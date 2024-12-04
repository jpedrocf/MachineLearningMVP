# MachineLearningMVP


Tentar localizar o reviewScoreClass com base nas outras métricas fornecidas, para checar quais métricas fazem um game ter bons reviews, colocar o que compõe o dataset, explicar que é uma reviewScoreClass é uma métrica criada, baseada na variável reviewScore


## Problem Definition
#### Objective:
The objective of this project is to develop a Machine Learning model capable of classifying a game's Review Score Class into three categories: Low, Medium, and High. This classification aims to identify and understand the key features that contribute to a game's evaluation.

## Problem Description
The problem involves analyzing game reviews (potentially sourced from gaming platforms, digital stores, or internal data). It is a multi-class classification problem, where the model is expected to categorize data based on a set of features provided in the dataset.

### Assumptions and Hypotheses:

#### Assumptions:

There exists a set of relevant features (such as gameplay, graphics, story, etc.) that directly influence the Review Score Class.
The Review Score Class is consistent and reliable, reflecting the general perception of a game's quality by a significant sample of users.

#### Hypotheses:

Games classified as "High" in Review Score Class possess specific feature combinations that distinguish them from "Low" or "Medium" games.
Features such as game genre, average playtime, cost, or release date may significantly impact the Review Score Class.


## Constraints or Conditions for Data Selection
Only games with recorded reviews available in a structured format will be included.
The dataset must include at least three distinct classes for the Review Score Class: Low, Medium, and High.
The number of records (games) must be sufficiently large to train and evaluate the Machine Learning model, ensuring representativeness for each class.
The data must include at least some quantitative and qualitative variables that are interpretable in the context of game reviews.
Data containing missing values or anomalies will be treated or discarded to avoid negatively affecting the model.


## Dataset Description

[Data Catalog](DataCatalog.md)
