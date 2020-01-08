# Deep Reinforcement Learning Udacity Nanodegree
## Project 2: Continuous Control problem
The [Unity ML-Agents toolkit](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Learning-Environment-Examples.md) contains the [Reacher Environment](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Learning-Environment-Examples.md#reacher) in which double-jointed arms have to move to target locations (see [video](https://www.youtube.com/watch?v=2N9EoF6pQyE)).

[//]: # (Image References)

[image1]: https://video.udacity-data.com/topher/2018/June/5b1ea778_reacher/reacher.gif "Trained Agents"

![image1]

### Project details

In a nutshell, we teach the robotic arms to follow the targets by the Deep Deterministic Policy Gradient method.

This environment rewards a reacher in the target location with +0.1. The vector observation space is 26 dimensional and the vector action space has 4 dimensions corresponding to the torque applicable to two joints. The environment is considered 'solved' when an average reward of +30 per episode is achieved. 

Due to the continuous action space, classical value-based methods are hard to apply. Instead, we solve the environment using the Deep Deterministic Policy Gradient (DDPG) method. This is a flavour of an actor-critic method, where the actor is trained to maximize the expected outcome as is predicted by the critic network. The twenty different robotic arms share their experiences and thus learn faster than a single actor.

I worked on this project as part of the [Deep Reinforcement Learning Udacity Nanodegree](https://www.udacity.com/course/deep-reinforcement-learning-nanodegree--nd893) and adapted the DDPG agent code from [Pendulum project in Udacity's Deep Reinforcement Learning Repository](https://github.com/udacity/deep-reinforcement-learning/tree/master/ddpg-pendulum)

## Getting Started

1. Set up your environment according to the instructions of the [DRLND GitHub repository](https://github.com/udacity/deep-reinforcement-learning#dependencies)

2. Clone this GitHub repository [continuouscontrol-DDPG](https://github.com/hullmann/continuouscontrol-DDPG)

3. Udacity provides a modified Unity environment. Please download the one matching your OS from the links below:
    - Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Linux.zip)
    - Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher.app.zip)
    - Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Windows_x86.zip)
    - Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Windows_x86_64.zip)

Place the file in the `continuouscontrol-DDPG/` folder (cloned in step 2.), and unzip the file. 

## Instructions
Follow the instructions in Continuous_Control.ipynb to train your agent or scroll to the bottom of the code to let the agent run based on pretrained weights.
