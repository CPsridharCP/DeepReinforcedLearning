# Project 3: Collaboration and Competition MADDPG

#### Pre Training --> Post Training
![](https://media.giphy.com/media/Q4fut2cCiHnxBISXqQ/giphy.gif)
![](https://media.giphy.com/media/RTbDwVdJddTIXxK7WR/giphy.gif)

### Introduction
This project solves for two agents to learn and play table-table tennis against each other. Implemented using MA-DDPG (Multi Agent Deep Deterministic Policy Gradient) algorithm. Each agent has two actor (local and target) and two critic (local and target) neural net models, and they share the replay buffer (experiences from the past - s a r s’ d).

Tennis Unity Environment provided by Udacity and is used for this project. (link to env below)

In this environment, two agents control rackets to bounce a ball over a net. If an agent hits the ball over the net, it receives a reward of +0.1. If an agent lets a ball hit the ground or hits the ball out of bounds, it receives a reward of -0.01. Thus, the goal of each agent is to keep the ball in play.
The observation space consists of 8 variables corresponding to the position and velocity of the ball and racket. Each agent receives its own, local observation. Two continuous actions are available, corresponding to movement toward (or away from) the net, and jumping. The task is episodic, and in order to solve the environment, your agents must get an average score of +0.5 (over 100 consecutive episodes, after taking the maximum over both agents). After each episode, we add up the rewards that each agent received (without discounting), to get a score for each agent. This yields 2 (potentially different) scores. We then take the maximum of these 2 scores. This yields a single score for each episode.

State/Observation size : 24 

Action space size : 2 

Number of Agents : 2 

Goal: The environment is considered solved, when the average (over 100 episodes) of those scores is at least +0.5.

### Getting Started

1. Clone the DRL Nanodegree learning repo : [click here](https://github.com/udacity/deep-reinforcement-learning#dependencies)

2. Download the environment from one of the links below. 
    - Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis_Linux.zip)
    - Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis.app.zip)
    - Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis_Windows_x86.zip)
    - Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis_Windows_x86_64.zip)

3. Place the file in the p3_collab-compet/ folder in the DRLND GitHub repository, and unzip (or decompress) the file.

4. Open Tennis.ipynb (located in the p3_collab-compet/ folder in the DRLND GitHub repository) and follow the instructions to retarin or test the trained weights.


### Learning Algorithm

MA-DDPG - Multi Agent Deep Deterministic Policy Gradient

MADDPG is an extension version of DDPG algorithm for multiple agents, an Actor-Critic algorithm that simultaneously learns a policy and an action-value function Q(s,a) for each agent. The actor takes a deterministic action following a policy and critic critics the actors action based on its action-value function.
Noise is added to the action intentionally to match up for a continuous action space use case through the output is deterministic.
 
Other helpful methods used to improve learning stability include:

Experience replay from memory, Local and Target networks for each Actor and Critic with a soft update feature, Gradient clipping at 1 to avoid parameter blow up, periodic learning, batch normalization. 

Hyperparamteres used and Network Architecture are discussed in the report. 
