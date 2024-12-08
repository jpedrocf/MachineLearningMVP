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


### Dataset Description

For a detailed description of each attribute in the dataset, including definitions, data types, and value ranges, refer to the [Data Catalog](DataCatalog.md).

# Notebook Workflow

## Data Cleaning and Management
- **Merging Datasets**:
  - Combined the `Players 23-24` and `Players Score 23-24` tables for a unified dataset.
- **Column Selection and Adjustment**:
  - Curated and reformatted columns to create a cleaner and more concise dataset.
- **Feature Creation**:
  - Generated new columns to enhance insights and improve the effectiveness of machine learning algorithms.
- **Handling Duplicates**:
  - Consolidated duplicate records for players who changed clubs, summing their variables to accurately reflect their full season performance.
- **Null Value Removal**:
  - Eliminated missing values to ensure data integrity and readiness for analysis.
- **Categorical Variable Encoding**:
  - Applied one-hot encoding to transform categorical variables into a format suitable for machine learning models.


## Data Analysis
- **Scatter Plot**:
  - Visualized relationships between key numerical features.
- **Heatmaps**:
  - Analyzed feature correlations and interactions to identify patterns and potential predictors.


## Target Definition
- **Target Exploration**:
  - Tested potential target variables using quartiles, absolute values, and clustering techniques to determine the most suitable target for prediction tasks.


## Model Testing
- **Feature Engineering**:
  - Enhanced features through data transformations and derivations to improve model performance.
- **Hyperparamer Tuning**
  - Conducted systematic testing and tuning of model hyperparameters to optimize results.
- **Pipelines**:
  - Integrated steps for:
    - **Data Transformation**:
      - Applied normalization (scaling to [0, 1]) and standardization (scaling to zero mean and unit variance) to compare performance across machine learning models.
    - **Model Workflow**:
      - Streamlined the modeling process to ensure reproducibility and efficiency.


## Machine Learning
- **Voting Classifier**:
  - Implemented a Voting Classifier with tuned hyperparameters to combine the strengths of multiple models.
- **Performance and Challenges**:
  - Achieved consistent results but identified the need for additional data to reach top-tier performance, given the limited sample size.









