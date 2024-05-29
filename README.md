# Real Time Cricket Match Outcome Prediction
## Introduction
We utilized a dataset of past T20 international matches from CRICSHEET and trained a deep neural network to provide the winning probability for teams after each ball of the game.

## Dataset
Dataset was collected from the [CRICSHEET](https://cricsheet.org/) webiste. Cricsheet provides access to ball by ball data for men and women Test matches, ODI, T20 internationals and all IPL seasons. The data is provided in YAML format. We took data for men T20 international matches, parsed it and generated a csv file with required attributes.

## Data Preprocessing
For each ball in a match a feature of ['team-batting', 'team-bowling', 'wicket-left', 'runs-scored', 'target-score', 'balls-bowled',
'batsman-score', 'nonstriker-score', 'batsman-balls-faced', 'nonstriker-balls-faced'] is created. And feature of a match will be a collection of the feature corresponding to each ball in the match. Match's feature is fed to model for training and prediction.

## Training
An LSTM neural network model is used for training. 
