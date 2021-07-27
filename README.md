# Using Deep Reinforcement Learning for Navigation
Navigation codes for the project Navigation submission.

# About the Project

The goal of the project is to train an agent to navigate in a world and collect as many yellow bananas as possible, as fast as it can. Also it should avoid collecting blue bananas as part of the challenge. 

To do that a reinforcement learning agent was trained. Specifically it was trained using a Deep Neural Network, with a technique called DQN, similar as was presented in the original DQN [paper](https://storage.googleapis.com/deepmind-media/dqn/DQNNaturePaper.pdf).

# Project Details

The environment is a **Unity Machine Learning Agents (ML-Agents)**, which is an open-source Unity plugin that enables games and simulations to serve as environments for training intelligent agents. In that environment an agent must be trained to collect as many yellow bananas as possible, while avoiding blue bananas because

- each yellow banana gives the agent a reward of +1;
- each blue banana gives the agent a reward of -1.

In that case the agent can select four actions in order to move around the simulated environment: left, right, forward and backward. To do that it receives from the environment a total of 37 features (which means that the state space is 37) containing the agent's velocity, along with ray-based perception of objects around the agent's forward direction.

**How to complete the task**: To solve the task, the agent must meet the criteria of achieving an average score of + 13 over 100 consecutive episodes.


# Ideas to Explore Later

Some ideas that could lead to improvements in the learning process are trying to:

- Use Double Q-Learning, as presented [here](https://arxiv.org/pdf/1509.06461). The idea is very similar the the DQN, but the Q-learning algorithm is known to overestimate action values under certain conditions and so double Q-learning could lead to better performance.


