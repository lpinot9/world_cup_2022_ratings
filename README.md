# WORLD CUP 2022 PLAYER RATINGS PROJECT

## Project objectives

Football and its huge mediatization and star system often overshadow some key players performances on the profit of big names, usually strikers positions.

Let's explore players' data on the biggest sport event to see if there is to some extent a justification to the inequalities of fame among players (outside football fans,  most followers during the world cup only know a handful of key players)

The goal of this project is :
- to explore and visualize players performance during the 2022 World Cun in Qatar
- to try rating the players on a scale of 0 to 100 and compare players by aggregated positions on the fields : Offensive players, Midfielders and Defensives players (goal keepers are excluded of the analysis)

## Sources

The data was found on [Kaggle](https://www.kaggle.com/datasets/swaptr/fifa-world-cup-2022-player-data)

Player ratings were built using weighted averages inspired by the video game FIFA (for instance to fairly compare offensive players, it is important to outline some performance depending on the position - a center forward does not have the same responsabilities as a winger and should not be valued the same way)

The dataset is git ignored and should be downloaded from Kaggle directly

## Project description

1. Data preparation

The prepatation and cleaning was made using Dataiku in order to produce the final data set in the folder 'clean_data'. Here is a summary of what was done :

- Joining of the different datasets using the column 'ranker' as a primary key
- Filtering : exlude goalkeepers, exclude players that played less than 180 minutes
- Column selection : or put differently getting rid of duplicated information and irrelvant information
- Aggregation of Data to have intersting categorical features :
  - Age was grouped into 4 categories
  =>  Prospects (up to 21),
      Youngsters (22 to 27),
      Confirmed (28 to 33),
      Veterans (from 33 upwards)


2. EDA

Exploratory Data Analysis was done in the notebook *aaa.ipynb*

3. Player Rating

The notebook *zzzz.ipynb* contains :

- The detailed steps from features transformation to the building of the ratings and the computing of weighed average

- The visualization of top performers by aggregated positions
