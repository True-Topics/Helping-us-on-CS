
![Types-of-Reinforcement-Learning](https://media.geeksforgeeks.org/wp-content/uploads/20241009151901458277/Types-of-Reinforcement-Learning.png)
## Types of Reinforcement Learning
There are two types of reinforcement learning: model-based and model-free.
### Model-Based Reinforcement Learning
With model-based reinforcement learning (RL), there’s a model that an agent uses to create additional experiences. Think of this model as a mental image that the agent can analyze to assess whether particular strategies could work.

Some of the advantages of this RL type are:
- It doesn’t need a lot of samples.
- It can save time.
- It offers a safe environment for testing and exploration.

The potential drawbacks are:
- Its performance relies on the model. If the model isn’t good, the performance won’t be good either.
- It’s quite complex.

### Model-Free Reinforcement Learning
In this case, an agent doesn’t rely on a model. Instead, the basis for its actions lies in direct interactions with the environment. An agent tries different scenarios and tests whether they’re successful. If yes, the agent will keep repeating them. If not, it will try another scenario until it finds the right one.

What are the advantages of model-free reinforcement learning?
- It doesn’t depend on a model’s accuracy.
- It’s not as computationally complex as model-based RL.
- It’s often better for real-life situations.

Some of the drawbacks are:
- It requires more exploration, so it can be more time-consuming.
- It can be dangerous because it relies on real-life interactions.

### Model-Based vs. Model-Free Reinforcement Learning: Example
Understanding model-based and model-free RL can be challenging because they often seem too complex and abstract. We’ll try to make the concepts easier to understand through a real-life example.

Let’s say you have two soccer teams that have never played each other before. Therefore, neither of the teams knows what to expect. At the beginning of the match, Team A tries different strategies to see whether they can score a goal. When they find a strategy that works, they’ll keep using it to score more goals. This is model-free reinforcement learning.

On the other hand, Team B came prepared. They spent hours investigating strategies and examining the opponent. The players came up with tactics based on their interpretation of how Team A will play. This is model-based reinforcement learning.

Who will be more successful? There’s no way to tell. Team B may be more successful in the beginning because they have previous knowledge. But Team A can catch up quickly, especially if they use the right tactics from the start.
## Reinforcement Learning Algorithms
A reinforcement learning algorithm specifies how an agent learns suitable actions from the rewards. RL algorithms are divided into two categories: value-based and policy gradient-based.
### Value-Based Algorithms
Value-based algorithms learn the value at each state of the environment, where the value of a state is given by the expected rewards to complete the task while starting from that state.
#### Q-Learning
This model-free, off-policy RL algorithm focuses on providing guidelines to the agent on what actions to take and under what circumstances to win the reward. The algorithm uses Q-tables in which it calculates the potential rewards for different state-action pairs in the environment. The table contains Q-values that get updated after each action during the agent’s training. During execution, the agent goes back to this table to see which actions have the best value.
#### Deep Q-Networks (DQN)
Deep Q-networks, or deep q-learning, operate similarly to q-learning. The main difference is that the algorithm in this case is based on neural networks.
#### SARSA
The acronym stands for state-action-reward-state-action. SARSA is an on-policy RL algorithm that uses the current action from the current policy to learn the value.
### Policy-Based Algorithms
These algorithms directly update the policy to maximize the reward. There are different policy gradient-based algorithms: REINFORCE, proximal policy optimization, trust region policy optimization, actor-critic algorithms, advantage actor-critic, deep deterministic policy gradient (DDPG), and twin-delayed DDPG.
#### Sources
- [Types of Reinforcement Learning - GeeksforGeeks](https://www.geeksforgeeks.org/types-of-reinforcement-learning/)
- [Reinforcement Learning: AI Algorithms, Types & Examples - OPIT](https://www.opit.com/magazine/reinforcement-learning-2/)