# Open-AI-gym-Frozen-Lake
This repository is one of my learning project for Reinforcement Learning(RL). It contains my codes of implementing Value Iteration and Policy Iteration in playing Frozen-Lake-v0 problem in OpenAI Gym.

## OpenAI Gym
Gym is a toolkit for developing and comparing reinforcement learning algorithms. It supports teaching agents everything from walking to playing games.

## Frozen Lake Problem
![image](https://user-images.githubusercontent.com/40629085/91283571-563e9a80-e7bd-11ea-97f3-d38ce4f700fa.png)

The agent controls the movement of a character in a grid world. Some tiles of the grid are walkable, and others lead to the agent falling into the water. Additionally, the movement direction of the agent is uncertain and only partially depends on the chosen direction. The agent is rewarded for finding a walkable path to a goal tile.

## Training the agent
An effective agent can be trained using 2 different algorithms: Value Iteration & Policy Iteration
### Value Iteration
Optimal state-value function(V*) is iteratively computed until convergence or maximum iteration. Then policy is extracted using this optimal value function. This usually has a much faster convergence speed than Policy Iteration.
### Policy Iteration
At each time of iteration, a policy is evaluated and a new state-value function(V) obtained from the policy. Then the policy is updated using V. The steps continue until convergence or maximum iteration. 
