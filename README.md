# MachineLearningMVP - Premier League 23/24 Tierlist of Offensive Players

## Problem Definition
#### Objective:

The objective of this work is to train a model capable of analyzing the features and determining whether a offensive Premier League player belongs to the high, medium or low tier. In future seasons, without access to official ratings, the model should be able to classify players solely based on their features. The training was conducted using a supervised learning approach.

## Problem Description


### Assumptions and Hypotheses:

#### Assumptions:



#### Hypotheses:

- Player features such as goals scored (Gls), assists (Ast), expected goals (xG), and expected assists (xAG) are strong indicators of a player’s tier. Players with higher values in these metrics are more likely to be classified in the "high" tier, while lower values are associated with the "low" tier.

- 


## Constraints or Conditions for Data Selection



## Dataset Description

For a detailed description of each attribute in the dataset, including definitions, data types, and value ranges, refer to the [Data Catalog](DataCatalog.md)








Assumptions:
Availability of Relevant Features:

It is assumed that the available player features (goals, assists, expected goals, minutes played, etc.) are indicative of their overall performance and can be used to classify players into high, medium, or low tiers.
Consistency of Player Behavior:

The performance of players in a given season is assumed to be representative of their abilities in future seasons, meaning their features (e.g., goals, assists, expected metrics) reflect their overall playing style and impact.
No External Rating Data:

The model will classify players without the use of external official ratings (like those from platforms such as Sofascore or Whoscored) in future seasons, relying solely on the players' features.
Supervised Learning Approach:

It is assumed that a supervised learning approach is appropriate for this task, and that sufficient labeled data (player features along with tier labels) is available for training the model.
Player Features Are Relevant:

It is assumed that the features being used (goals, assists, xG, xA, minutes played, etc.) are predictive of the player’s tier and will allow the model to make accurate predictions.
Balanced Dataset:

The dataset is assumed to have a balanced distribution of players across high, medium, and low tiers. If the dataset is imbalanced, performance may suffer, and adjustments will need to be made.
Player Tier Classification:

It is assumed that the tier classification (high, medium, low) is based on an objective scoring system, even though it may rely on subjective judgments. For instance, tiers might be assigned based on quantifiable metrics like goals per match, expected goals, assists, or other performance-related features.
Feature Engineering:

It is assumed that the relevant features have been preprocessed and transformed into a usable format, with necessary normalization and handling of missing values to avoid introducing bias into the model.




Hypothesis 2:

Minutes played (Min) could have a significant impact on tier classification. Players with a higher number of minutes played are more likely to be in the "high" tier, as they have more opportunities to impact the game. Conversely, players with fewer minutes might be in the "low" tier due to limited playtime.
Hypothesis 3:

The correlation between expected goals (xG) and actual goals (Gls) will help distinguish high-performing players. High-tier players will have a higher correlation between these metrics, as they convert expected goals into actual goals more effectively.
Hypothesis 4:

Consistency of performance over the course of a season (i.e., consistent contributions in goals, assists, and minutes) will be a significant indicator. High-tier players should show more consistent performance, while low-tier players might have more variable outputs.
Hypothesis 5:

Certain positional features (e.g., Forward, Midfielder) will influence the classification. For example, forwards might have a higher chance of being in the "high" tier due to their greater involvement in scoring, while midfielders and defenders might have a lower average tier unless they contribute significantly in other areas.
Hypothesis 6:

There is a threshold for tier classification based on specific feature values. For example, a player scoring more than X goals and having an assist rate above Y may automatically classify them in the high tier, while below those thresholds may place them in the medium or low tier.
Hypothesis 7:

Player age and injury history might indirectly affect a player's tier, with younger, fit players more likely to perform at higher tiers and older or injury-prone players possibly performing at lower tiers.
