# DATA 607 Project 1 – Chess Tournament

This repository contains the approach and supporting files for DATA 607 Project 1.

## Project Objective

The objective is to transform the semi-structured chess tournament results contained in `tournamentinfo.txt` into a structured CSV dataset using R.

The final dataset will contain one record for each of the 64 players and the following variables:

- Player name
- State or province
- Total tournament points
- Pre-tournament rating
- Average pre-tournament rating of the opponents faced

The average opponent rating will be calculated by extracting each player's numbered opponents, matching those numbers with the corresponding tournament players, and averaging their pre-tournament ratings.

## Current Submission

This repository currently contains the Project 1 Approach, which documents:

- The original data source
- The structure of the tournament text file
- The proposed data-transformation process
- The data dictionary
- The validation plan
- The expected CSV output

The complete transformation code, exploratory analysis, validation results, and final CSV file will be added during the Code Base phase of the project.

## Files

- `DATA607-Project1-Chess-Tournament-Approach.qmd`: Quarto source document
- `DATA607-Project1-Chess-Tournament-Approach.html`: Rendered approach report
- `tournamentinfo.txt`: Original tournament data provided for the assignment
- `DATA607-Project1-Chess-Tournament.Rproj`: RStudio project file

## Expected Output

The completed project will generate:

`chess_tournament_results.csv`

The file will contain 64 player records and five analytical columns.

The first expected record is:

```text
player_name,state,total_points,pre_rating,average_opponent_pre_rating
Gary Hua,ON,6.0,1794,1605
```

## Published Approach

The rendered approach is available on RPubs:

[DATA 607 Project 1 – Chess Tournament Approach](https://rpubs.com/howtwo3/data607-project1-chess-tournament-approach)

## Repository

[DATA607 Project 1 – Chess Tournament](https://github.com/howtwo388-cyber/DATA607-Project1-Chess-Tournament)

## Tools

- R
- Quarto
- RStudio
- Git and GitHub
- `readr`
- `dplyr`
- `stringr`
- `ggplot2`
- `skimr`
- `knitr`

## AI Use

ChatGPT was used to help interpret the assignment requirements, organize the planned approach, improve the English writing, and provide coding guidance. I will run the code, review the results, validate the final dataset, and confirm the conclusions myself.
