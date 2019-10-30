# Project - BipedalWalker with A2C, Vectorized Environment


### Introduction

Solving the environment require an average total reward of over 300 over 100 consecutive episodes.
Training of BipedalWalker is considered as [difficult task](https://ctmakro.github.io/site/on_learning/rl/bipedal.html), in particular, it is very difficult to train BipedalWalker by DDPG and PPO (with one agent). In this directory we solve the environment 
in **1646** (resp. **2188**) episodes by usage of the __A2C__ algorithm with RMSprop (resp. Adam) optimizer, see [Understanding Actor Critic Methods and A2C](https://towardsdatascience.com/understanding-actor-critic-methods-931b97b6df3f).
For other solutions (based on the single agent) see
[BipedalWalker-TD3](https://github.com/Rafael1s/Deep-Reinforcement-Learning-Udacity/tree/master/BipedalWalker-TwinDelayed-DDPG%20(TD3))
and [BipedalWalker-SAC](https://github.com/Rafael1s/Deep-Reinforcement-Learning-Udacity/tree/master/BipedalWalker-Soft-Actor-Critic).

![](images/bwalker_a2c.png)     

### Requirement

* [python 3.7](https://www.python.org) 
* [pytorch 1.0.1](https://pytorch.org/)
* [gym 0.13.1](https://github.com/openai/gym)


### Training the Agent
We train the agent to understand that it can use information from its surroundings to inform the next best action.    
The score 300.5 was achieved    

* in the episode **1646** after training **11 hours 44 minutes**.
lr = **0.001**, optimizer = **RMSprop**.

![](images/plot_a2c_1646epis.png) 

* in the episode **2188** after training **14 hours 43 minutes**.
lr = **0.0005**, optimizer = **Adam**.

![](images/plot_a2c_2188epis.png) 

### Other BipedalWalker projects:

* [BipedalWalker, TD3](https://github.com/Rafael1s/Deep-Reinforcement-Learning-Udacity/tree/master/BipedalWalker-TwinDelayed-DDPG%20(TD3))    
* [BipedalWalker, SAC](https://github.com/Rafael1s/Deep-Reinforcement-Learning-Udacity/tree/master/BipedalWalker-Soft-Actor-Critic)    
* [BipedalWalker, PPO, Vectorized Env](https://github.com/Rafael1s/Deep-Reinforcement-Learning-Udacity/tree/master/BipedalWalker-PPO-VectorizedEnv)  

### Credit   

Most of the code is based on the Udacity code, and Ilya Kostrikov's code (https://github.com/ikostrikov).