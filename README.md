# drlnd_tennis
Project 3 of the Deep Reinforcement Learning Nanodegree on Udacity

## Introduction
Train an agent to play tennis within the [Tennis environment by unity](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Learning-Environment-Examples.md#tennis) using a Multi-Agent DDPQ algorithm.

## How it works 

![Tennis](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/images/tennis.png)
Picture taken from [official site](https://github.com/Unity-Technologies/ml-agents).

Description taken from the Udacity course:
In this environment, two agents control rackets to bounce a ball over a net. If an agent hits the ball over the net, it receives a reward of +0.1. If an agent lets a ball hit the ground or hits the ball out of bounds, it receives a reward of -0.01. Thus, the goal of each agent is to keep the ball in play.

The observation space consists of 8 variables corresponding to the position and velocity of the ball and racket. Each agent receives its own, local observation. Two continuous actions are available, corresponding to movement toward (or away from) the net, and jumping.

The task is episodic, and in order to solve the environment, your agents must get an average score of +0.5 (over 100 consecutive episodes, after taking the maximum over both agents). Specifically,
 - After each episode, we add up the rewards that each agent received (without discounting), to get a score for each agent. This yields 2 (potentially different) scores. We then take the maximum of these 2 scores.
 - This yields a single score for each episode.
 
The environment is considered solved, when the average (over 100 episodes) of those scores is at least +0.5.


### Getting Started / Setup

1. Set up a python environment including python 3.6+, numpy, matplotlib, torch.

2. Follow the steps in [here](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Installation.md) to install the Unity ML-Agents Toolkit.

3. Clone this repository via `git clone https://github.com/kheimpel/drlnd_tennis.git`

4. Download the Banana Navigation environment from one of the links below.  Select the environment which matches your operating system:
    - Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis_Linux.zip)
    - Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis.app.zip)
    - Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis_Windows_x86.zip)
    - Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis_Windows_x86_64.zip)
    
5. Place the file in the folder of the repository


### Instructions

Follow the instructions in `Tennis_Solution.ipynb` to train your own agent!

You can also use the pretrained agents (actor and critic) `checkpoint_actor_success.pth` + `checkpoint_critic_success.pth` (= pytorch models) which successfully solved the environment (in ~1092 steps).

### Notes
We make extensive use of code that was provided within previous exercises of the Udacity Deep RL Nanodegree (especially the plain DDPQ implementation).
