# Random Walk Exercise and Temporal Difference Learning

## Random Walk Exercise

The random walk exercise is a foundational concept in reinforcement learning and probability theory. It involves an agent that starts at a given state and moves randomly between states based on defined probabilities. The primary objective of the random walk is to analyze how the agent's position changes over time and to understand the expected outcomes of its transitions.

In the basic setup of a random walk:
- The agent can move to neighboring states with equal probability.
- Boundaries may be defined, and rules established for what happens when the agent reaches the boundaries.

### Applications
This exercise serves as a simplified model for various real-world scenarios, such as stock prices in finance or decision-making processes in uncertain environments.

## Temporal Difference Learning (TD Learning)

Temporal Difference Learning is a key concept within reinforcement learning that combines ideas from dynamic programming and Monte Carlo methods. It allows agents to learn directly from raw experience without needing a model of the environment.

Key aspects of TD Learning include:
1. **Learning from Episodes**: Agents adjust their predictions based on the difference between predicted rewards and actual outcomes as new data is received over time.
2. **Bootstrapping**: TD methods update value estimates based partially on other current estimates rather than waiting for the final outcome, which allows for more efficient learning.

### TD(0) Algorithm
One of the simplest forms of TD learning is the TD(0) algorithm, which updates the value of the current state by looking at the immediate reward and the value of the next state. The update rule can be expressed as:
\[ V(S_t) \leftarrow V(S_t) + \alpha(R_{t+1} + \gamma V(S_{t+1}) - V(S_t)) \]
where:
- \( V(S_t) \) is the value of the current state.
- \( \alpha \) is the learning rate.
- \( R_{t+1} \) is the reward received after transitioning to the next state.
- \( \gamma \) is the discount factor, which represents the importance of future rewards.

By continually iterating this process, the agent can effectively learn the value function and make better decisions.