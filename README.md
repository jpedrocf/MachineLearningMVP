# MachineLearningMVP - Premier League 23/24 Tierlist of Offensive Players

## Problem Definition
#### Objective:

The objective of this work is to train a model capable of analyzing the features and determining whether a offensive Premier League player belongs to the high, medium or low tier. In future seasons, without access to official ratings, the model should be able to classify players solely based on their features. The training was conducted using a supervised learning approach.

## Problem Description


### Assumptions and Hypotheses:

#### Assumptions:

- It is assumed that the available player features (goals, assists, expected goals, minutes played, etc.) are indicative of their overall performance and can be used to classify players into high, medium, or low tiers.

- The model will classify players without the use of external official ratings (like those from platforms such as Sofascore or Whoscored) in future seasons, relying solely on the players' features.

- It is assumed that a supervised learning approach is appropriate for this task, and that sufficient labeled data (player features along with tier labels) is available for training the model.

- It is assumed that the features being used (goals, assists, xG, xA, minutes played, etc.) are predictive of the player’s tier and will allow the model to make accurate predictions.


#### Hypotheses:

- Player features such as goals scored (Gls), assists (Ast), expected goals (xG), and expected assists (xAG) are strong indicators of a player’s tier. Players with higher values in these metrics are more likely to be classified in the "high" tier, while lower values are associated with the "low" tier.

- Minutes played (Min) could have a significant impact on tier classification. Players with a higher number of minutes played are more likely to be in the "high" tier, as they have more opportunities to impact the game. Conversely, players with fewer minutes might be in the "low" tier due to limited playtime.

- The correlation between expected goals (xG) and actual goals (Gls) will help distinguish high-performing players. High-tier players will have a higher correlation between these metrics, as they convert expected goals into actual goals more effectively. I created a column named Effectiveness that calculates that proportion.


## Constraints or Conditions for Data Selection



## Dataset Description

For a detailed description of each attribute in the dataset, including definitions, data types, and value ranges, refer to the [Data Catalog](DataCatalog.md)





