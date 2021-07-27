# Using Deep Reinforcement Learning for Navigation
Navigation codes for the project Navigation submission.

## About the Project

The goal of the project is to train an agent to navigate in a world and collect as many yellow bananas as possible, as fast as it can. Also it should avoid collecting blue bananas as part of the challenge. 

To do that a reinforcement learning agent was trained. Specifically it was trained using a Deep Neural Network, with a technique called DQN, similar as was presented in the original DQN [paper](https://storage.googleapis.com/deepmind-media/dqn/DQNNaturePaper.pdf).

## What is Reinforcement Learning

From [deepsense.ai](https://deepsense.ai/what-is-reinforcement-learning-the-complete-guide/), we have that 

> Reinforcement learning is the training of machine learning models to make a sequence of decisions. The agent learns to achieve a goal in an uncertain, potentially complex environment. In reinforcement learning, an artificial intelligence faces a game-like situation. The computer employs trial and error to come up with a solution to the problem. To get the machine to do what the programmer wants, the artificial intelligence gets either rewards or penalties for the actions it performs. Its goal is to maximize the total reward.
Although the designer sets the reward policy–that is, the rules of the game–he gives the model no hints or suggestions for how to solve the game. It’s up to the model to figure out how to perform the task to maximize the reward, starting from totally random trials and finishing with sophisticated tactics and superhuman skills. By leveraging the power of search and many trials, reinforcement learning is currently the most effective way to hint machine’s creativity. In contrast to human beings, artificial intelligence can gather experience from thousands of parallel gameplays if a reinforcement learning algorithm is run on a sufficiently powerful computer infrastructure.

## Project Details

The environment is a **Unity Machine Learning Agents (ML-Agents)**, which is an open-source Unity plugin that enables games and simulations to serve as environments for training intelligent agents. In that environment an agent must be trained to collect as many yellow bananas as possible, while avoiding blue bananas because

- each yellow banana gives the agent a reward of +1;
- each blue banana gives the agent a reward of -1.

In that case the agent can select four actions in order to move around the simulated environment: left, right, forward and backward. To do that it receives from the environment a total of 37 features (which means that the state space is 37) containing the agent's velocity, along with ray-based perception of objects around the agent's forward direction.

**How to complete the task**: To solve the task, the agent must meet the criteria of achieving an average score of + 13 over 100 consecutive episodes.

### Environment Set Up

The project environment is similar to, but not identical to the Banana Collector environment on the [Unity ML-Agents GitHub page](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Learning-Environment-Examples.md#banana-collector).

**Note:** The Unity ML-Agent team frequently releases updated versions of their environment. I'm are using the v0.4 interface. To avoid any confusion, please use the workspace provided here or work with v0.4 locally.




## Ideas to Explore Later

Some ideas that could lead to improvements in the learning process are trying to:

- Use Double Q-Learning, as presented [here](https://arxiv.org/pdf/1509.06461). The idea is very similar the the DQN, but the Q-learning algorithm is known to overestimate action values under certain conditions and so double Q-learning could lead to better performance.


