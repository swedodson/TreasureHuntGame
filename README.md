# TreasureHuntGame
Machine learning program using Q-training algorithm

The theme of this project is a popular treasure hunt game in which the player needs to find the treasure before the pirate does. The pirate will try to find the optimal path to the treasure using deep Q-learning. 

The first class, TreasureMaze.py, represents the environment, which includes a maze object defined as a matrix. The second class, GameExperience.py, stores the episodes – that is, all the states that come in between the initial state and the terminal state. This is later used by the agent for learning by experience, called "exploration". 

The pirate agent can move in four directions: left, right, up, and down. While the agent primarily learns by experience through exploitation, often, the agent can choose to explore the environment to find previously undiscovered paths. This is called "exploration" and is defined by epsilon. This value is typically a lower value such as 0.1, which means for every ten attempts, the agent will attempt to learn by experience nine times and will randomly explore a new path one time. The goal of the deep Q-learning implementation is to find the best possible navigation sequence that results in reaching the treasure cell while maximizing the reward.
