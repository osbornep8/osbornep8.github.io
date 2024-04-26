---
title: "Interactive RPS Game with ML"
excerpt: "Challenge an ML model that adapts to your strategy in Rock, Paper, Scissors—powered by a Markov Chain.<br/><img src='/images/RPS.png'>"
collection: portfolio
---

This game uses Python to run in your terminal. It consists of 2 rounds:

1. Trial Round: A series of 6-8 rounds to quickly develop the Markov model so try to as abstract in your choices. The computer's choices in this round are simply based on random choices.

2. Main Game: In this round, you have 3 (modifiable) lives, you are now playing against the Markov Model developed based on your earlier pattern of play in the Trial Round.

The goal of this game was to simulate the players' strategy using an initial trial round and then use this to play against the player by playing the opposite move as the one predicted from the Markov model. Additionally, the player's moves are also periodically updated during the main game to improve prediction accuracy.

There are also some additional code blocks included to prevent overfitting of the model and maintain some randomness of choice.

You can view the code [here](https://github.com/osbornep8/RPS_with_Markov_Chain_Prediction)
