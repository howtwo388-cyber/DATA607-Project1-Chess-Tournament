# DATA 607 Project 1 – Chess Tournament

This repository contains the complete code, data transformation, validation, exploratory analysis, and deliverables for DATA 607 Project 1.

## Project Objective

The objective of this project is to transform the semi-structured chess tournament cross-table in `tournamentinfo.txt` into a tidy CSV dataset using R and Quarto.

The final dataset contains one record for each of the 64 tournament players and the following variables:

- Player name
- State or province
- Total tournament points
- Pre-tournament rating
- Average pre-tournament rating of the opponents faced

## Data Transformation

The Quarto code:

1. Reads the original tournament text file.
2. Identifies the two lines associated with each player.
3. Extracts player names, states, points, and pre-tournament ratings.
4. Extracts opponent pairing numbers from the seven tournament rounds.
5. Excludes special results that do not identify an opponent.
6. Matches each opponent number with the corresponding player's pre-rating.
7. Calculates each player's average opponent pre-rating.
8. Validates the transformed dataset.
9. Exports the final results as a CSV file.

## Validation Results

The completed dataset passed the following checks:

- 64 player records
- Five required analytical variables
- No missing required values
- No duplicate pairing numbers
- No invalid opponent references
- Successful CSV read-back validation
- Gary Hua's average opponent pre-rating equals `1605`

## Exploratory Analysis

The tournament data produced the following summary:

- Number of players: 64
- Mean pre-tournament rating: 1378.5
- Median pre-tournament rating: 1407
- Minimum pre-tournament rating: 377
- Maximum pre-tournament rating: 1794
- Mean opponent pre-rating: 1378.6

The exploratory visualization indicates that players with higher pre-tournament ratings generally faced stronger opponents.

## Repository Files

- `tournamentinfo.txt`: Original tournament cross-table
- `DATA607-Project1-Chess-Tournament-Approach.qmd`: Approach source document
- `DATA607-Project1-Chess-Tournament-Approach.html`: Rendered approach
- `DATA607-Project1-Chess-Tournament-Code-Base.qmd`: Complete reproducible code
- `DATA607-Project1-Chess-Tournament-Code-Base.html`: Rendered code-base report
- `chess_tournament_results.csv`: Final transformed dataset
- `DATA607-Project1-Chess-Tournament.Rproj`: RStudio project file

## Expected First Record

```text
player_name,state,total_points,pre_rating,average_opponent_pre_rating
Gary Hua,ON,6,1794,1605
```

## Published Reports

- [Project 1 Approach](https://rpubs.com/howtwo3/data607-project1-chess-tournament-approach)
- [Project 1 Code Base](https://rpubs.com/howtwo3/ata607-project1-chess-tournament-code-base)

## GitHub Repository

[DATA607 Project 1 – Chess Tournament](https://github.com/howtwo388-cyber/DATA607-Project1-Chess-Tournament)

## Tools and Packages

- R
- Quarto
- RStudio
- Git and GitHub
- `readr`
- `dplyr`
- `stringr`
- `ggplot2`
- `knitr`

## AI Use

ChatGPT was used to help interpret the assignment requirements, organize the workflow, improve the English writing, explain the tournament cross-table structure, and provide coding guidance. I ran the code, reviewed the transformed data, validated the results, and confirmed the conclusions myself.
