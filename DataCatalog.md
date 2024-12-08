# Data Catalog

About the final dataset (with merge and created features), used for the machine learning

| Column          | Type    | Feature/Target | Description                                                                 |
|-----------------|---------|----------------|-----------------------------------------------------------------------------|
| Starts          | Integer | Feature        | Number of matches the player started.                                       |
| Min             | Float   | Feature        | Total minutes played by the player.                                         |
| 90s             | Float   | Feature        | The equivalent of 90-minute matches played by the player.                   |
| Gls             | Float   | Feature        | Total number of goals scored by the player.                                 |
| Ast             | Float   | Feature        | Total number of assists made by the player.                                 |
| xAG             | Float   | Feature        | The expected number of assists from the player's passes.                    |
| Gls+Ast         | Float   | Feature        | Total number of goals and assists combined.                                 |
| xAst+xG         | Float   | Feature        | Total of non-penalty expected goals and expected assists.                   |
| Pos_FW          | Boolean | Feature        | Whether the player is a forward (`True` if yes, `False` if not).             |
| Pos_MF          | Boolean | Feature        | Whether the player is a midfielder (`True` if yes, `False` if not).         |
| Category Cluster| String  | Target         | The tier category for the player, with possible values: `Low Tier`, `Mid Tier`, `Top Tier`.|




About the Premier League Players 23/24 Dataset

This dataset contains detailed data on all footballers from the 2023/24 premier league season



| Column                         | Type    | Description                                                            |
|--------------------------------|---------|------------------------------------------------------------------------|
| Player                         | String  | The name of the player.                                                |
| Nation                         | String  | The player's nationality.                                              |
| Pos                            | String  | The player's position (e.g., forward, midfielder, defender).           |
| Age                            | Integer | The player's age.                                                      |
| MP (Minutes Played)            | Integer | Total minutes played by the player.                                    |
| Starts                         | Integer | Number of matches the player started.                                  |
| Min (Minutes)                  | Integer | Total minutes played by the player (this might be the same as MP).    |
| 90s (90s Played)               | Float   | The equivalent of 90-minute matches played by the player.              |
| Gls (Goals)                    | Integer | Total number of goals scored by the player.                            |
| Ast (Assists)                  | Integer | Total number of assists made by the player.                            |
| G+A (Goals + Assists)          | Integer | Total number of goals and assists combined.                            |
| G-PK (Goals - Penalty Kicks)   | Integer | Total number of goals scored excluding penalty kicks.                  |
| PK (Penalty Kicks)             | Integer | Number of penalty goals scored by the player.                         |
| PKatt (Penalty Kicks Attempted)| Integer | Number of penalty kicks attempted by the player.                      |
| CrdY (Yellow Cards)           | Integer | Number of yellow cards received by the player.                        |
| CrdR (Red Cards)              | Integer | Number of red cards received by the player.                           |
| xG (Expected Goals)           | Float   | The expected number of goals from the player's shots.                  |
| npxG (Non-Penalty Expected Goals) | Float | Expected goals excluding penalties.                                  |
| xAG (Expected Assists)         | Float   | The expected number of assists from the player's passes.              |
| npxG+xAG (Non-Penalty xG + xAG) | Float | Total of non-penalty expected goals and expected assists.              |
| PrgC (Progressive Carries)    | Integer | Number of times the player carried the ball forward.                  |
| PrgP (Progressive Passes)     | Integer | Number of passes made by the player that moved the ball forward.      |
| PrgR (Progressive Runs)       | Integer | Number of times the player made runs forward with the ball.           |


About the Players Sofascore Score dataset

This dataset contains Team, Player and SofascoreScore data, used to merge with the other dataset


| Column                         | Type    | Description                                                            |
|--------------------------------|---------|------------------------------------------------------------------------|
| Player                         | String  | The name of the player.                                                |
| Team                           | String  | The player's team.                                                     |
| SofascoreScore                 | Float   | The player's Sofascore Score, based on the 23/24 Premier League season.|
