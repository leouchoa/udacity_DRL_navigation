# Description

This document is a report describing the learning algorithm and details of implementation, along with ideas for future work.

# Algorithm: DQN and Q-Learning

The algorithm used is called `DQN`, where a neural network is used is to implement the `Q-Learning` Algorithm. The `Q-Learning` algorithm attempts to estimate action-value pairs in order to maximize the expected total reward and, therefore, to obtain the optimal policy for the given task. 

The `Q-Learning` algorithm belongs to class of value-based methods and 


$$ \displaystyle Q^{new}(s_{t},a_{t})\leftarrow \underbrace {Q(s_{t},a_{t})} _{\text{old value}}+\underbrace {\alpha } _{\text{learning rate}}\cdot \overbrace {{\bigg (}\underbrace {\underbrace {r_{t}} _{\text{reward}}+\underbrace {\gamma } _{\text{discount factor}}\cdot \underbrace {\max _{a}Q(s_{t+1},a)} _{\text{estimate of optimal future value}}} _{\text{new value (temporal difference target)}}-\underbrace {Q(s_{t},a_{t})} _{\text{old value}}{\bigg )}} ^{\text{temporal difference}} $$
