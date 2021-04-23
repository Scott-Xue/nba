# nba
## Introduction
Every season in the NBA, players move teams, get traded, retire, get cut, etc. There are many reasons for player movements, such as teams wanting good value players to compete for championships, players wanting to change teams, and many more. There are many ways to analyze this phenomenon, but I would like to take two approaches: a churn model (a player leaving a team during or at the end of a season is considered a player churn. Using the usual scenario where churn is used, a team is the subscription/business, and the player the consumer) and a stochastic process model that attempts to model end-of-season player transitions as a markov process (a player's transition probabilities to other teams is dependent only on the current status of said player and the other teams).

## Data
The primary data im using is from stats.nba.com through the nba_api library. It would be interesting to consider using external data sources such as media reports and social media chatter, but for now that is out of scope.
    - NBA seasons 1997-98 to 2020-21
    - 