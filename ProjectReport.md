# Project Report

This projects implements DQN to train an agent to pick up as many yellow bananas as possible while avoiding blue bananas.  

## Learning algorithm Goal

The goal of the D Q-Learning agent is to decide which actions to take within the environment to maximize reward. Since the effects of possible actions aren't known in advance, the optimal policy must be discovered by interacting with the environment and recording observations. Therefore, the agent "learns" the policy through a process of trial-and-error that iteratively maps various environment states to the actions that yield the highest reward.

## Hyperparameter 

The following hyperparameters are selected for the training: 

* number of episodes = 1700 
    - The number of episodes was a heuristic from seeing how previous runs performed.The final model solved the problem (average score of 13 over 100 episodes) at episode 432.

* max timesteps = 1000 
    - The max timesteps at 2000 was in an attempt to not cut-off well-performing agents too early.

* epsilon max = 1.0

* epsilon min = 0.01

* epsilon decay rate = 0.995



## Plot of Rewards
The plot below shows the rewards acquired by the agent over the 1700 episodes:
![Score per episode](score_per_episode_plot.png?raw=true "Rewards over Episodes")


## Future Improvements 
I would like to explore other algorthm like Dueling Q learning, Double Deep Q-Network then compare their performance with DQN.

I would also like to implement hyperparameter tuning of the model parameter to investigate how they affect the agent performance.
