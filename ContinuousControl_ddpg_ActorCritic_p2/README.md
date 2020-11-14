# Continuous Control with Reinforcement Learning

### The Environment
In this environment, a double-jointed arm can move to target locations. A reward of +0.1 is provided for each step that the agent's hand is in the goal location. Thus, the goal of your agent is to maintain its position at the target location for as many time steps as possible.

The observation space consists of 33 variables corresponding to position, rotation, velocity, and angular velocities of the arm. Each action is a vector with four numbers, corresponding to torque applicable to two joints. Every entry in the action vector is a number between -1 and 1.

State Size, Action Size, #of Agents = 33, 4, 20

### Goal
The environment is considered solved, when the average (over 100 episodes) of those average scores (all 20 agents) is at least +30.

### Getting Started
1. Clone the DRL Nanodegree learning repo : [click here](https://github.com/udacity/deep-reinforcement-learning#dependencies) and follow  instructions in readme to install/create conda environment and dependencies.

2. For this project, you will not need to install Unity - this is because the environment is already built for you, and you can download it from one of the links below. You need only select the environment that matches your operating system:

##### Version 1: One (1) Agent

Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher_Linux.zip)

Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher.app.zip)

Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher_Windows_x86.zip)

Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher_Windows_x86_64.zip)

##### Version 2: Twenty (20) Agents | This is the version I have used.

Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Linux.zip)

Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher.app.zip)

Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Windows_x86.zip)

Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Windows_x86_64.zip)

3. Place the file in the p2_continuous-control/ folder in the DRLND GitHub repository, and unzip (or decompress) the file.


