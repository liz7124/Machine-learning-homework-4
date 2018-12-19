# Homework 4 - Machine Learning
This repository provide answer for machine learning class homework 4 (Final Exam). The goal is to train agent to play **Grid World** using Monte-Carlo, SARSA, and Q-Learning. This code is modification from [RLCode Reinforcement Learning](https://github.com/rlcode/reinforcement-learning).

## Monte-Carlo
The Monte Carlo method for reinforcement learning learns directly from episodes of experience.
We don’t do an update after every action, but rather after every episode.

This program has 2 class: `Env` for environment and `MCAgent` for the agent.
When start the program, it will inisiate the starting value for the agent, reward, state, environment. In this code, it will run until 1000 episode. On each episode, the program will calculate the value of each grid, predict the next state, and calculate the reward. If the rectangle successful to reach the circle or the rectangle hit the triangle, it will end and move to next episode.

Using Monte-Carlo algorithm, the time that needed to become converge state is vary every time we run it. In earlier episode, the agent will moves at random. As it gets reward, it will learn what to do. Because it is reinforcement learning, the agent does many exploration in the beginning. Agent find good strategy by chance and learn the strategy. Reward is given from the environment. According to the environment, the agent can get different reward even if it is in the same state and does the same action.

## SARSA
When run SARSA if we are unlucky, the rectangle will stuck between the minus value, and it will takes long time to converge.


## Q-Learning