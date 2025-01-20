The K-armed bandit problem in reinforcement learning involves an agent choosing from K different actions or options, each with an unknown reward distribution. The goal is to maximize the total reward over time by selecting actions that yield the highest rewards. Each action has an associated expected reward, denoted as q∗(a)q^*(a), which is the mean reward for that action.
### Key Concepts:
1. **Action and Reward**: At each time step, the agent selects an action AtA_t, which results in a reward RtR_t based on the chosen action's reward distribution.
2. **True Action Value**: The value of an action aa, denoted q∗(a)q^*(a), is the expected reward when that action is chosen: q∗(a)=E\[Rt∣At=a]q^*(a) = E\[R_t | A_t = a].
3. **Estimated Action Value**: The agent maintains an estimate of each action's value Qt(a)Q_t(a), which may differ from the true value q∗(a)q^*(a) because the agent does not initially know the true rewards of the actions.
4. **Exploitation vs. Exploration**:
    - **Exploitation**: The agent selects the action that it believes will give the highest reward, based on its current estimates.
    - **Exploration**: The agent selects actions it hasn't tried as much in order to improve its estimates of their values.
### Conflict:
The challenge lies in balancing **exploration** (gathering information about all actions) and **exploitation** (choosing the best-known action based on current knowledge). Although exploitation maximizes short-term rewards, exploration can lead to better long-term rewards by revealing better actions that are not immediately obvious.
### Simple Methods:
While sophisticated methods for balancing exploration and exploitation can make assumptions about stationarity and prior knowledge, simple methods like the **ε-greedy algorithm** are often used. In **ε-greedy**, the agent usually selects the greedy (best-known) action but with a small probability (ε) chooses a random action to explore other possibilities.

These methods aim to ensure that exploration does not entirely give way to exploitation, preventing the agent from getting stuck in suboptimal choices.

In summary, the K-armed bandit problem highlights the challenge of balancing exploration and exploitation in reinforcement learning, where exploration can lead to discovering better long-term strategies, while exploitation provides immediate rewards.
#### Sources
- Reinforcement Learning An Introduction by Sutton, Richard S., Barto, Andrew G.