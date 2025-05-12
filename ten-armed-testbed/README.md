# 🎰 Ten-Armed Testbed – Reinforcement Learning Experiments

This project implements the classic 10-armed bandit testbed from Sutton and Barto’s *Reinforcement Learning: An Introduction*. It serves as a foundational environment for experimenting with various action-selection strategies in reinforcement learning.

---

## 📚 Overview

The 10-armed testbed simulates a scenario where an agent must choose between 10 different actions (or "arms") at each time step. Each arm provides a reward drawn from a stationary probability distribution unique to that arm. The agent's objective is to maximize the cumulative reward over time by learning the optimal action-selection strategy.

---

## 🧪 Experimental Setup

- **Bandit Problems**: 2000 independent 10-armed bandit problems are generated. For each problem:
  - The true action values \( q^*(a) \) for each arm \( a \in \{1, ..., 10\} \) are sampled from a normal distribution \( \mathcal{N}(0, 1) \).
  - When an action \( A_t \) is selected at time \( t \), a reward \( R_t \) is drawn from \( \mathcal{N}(q^*(A_t), 1) \).

- **Evaluation Metrics**:
  - **Average Reward**: The mean reward obtained over time, averaged across all runs.
  - **Percentage of Optimal Action**: The proportion of times the agent selects the optimal action (the one with the highest \( q^*(a) \)) at each time step.

---

## ⚙️ Implemented Algorithms

The project explores and compares the performance of the following action-selection strategies:

1. **Greedy**: Always selects the action with the highest estimated value.
2. **ε-Greedy**: With probability ε, selects a random action (exploration); otherwise, selects the best-known action (exploitation).
3. **UCB (Upper Confidence Bound)**: Selects actions based on both their estimated value and the uncertainty (confidence bounds) around those estimates.
4. **Optimistic Initial Values**: Encourages exploration by initializing action-value estimates optimistically high.
5. **GBA (Gradient Bandit Algorithm)**: Uses a softmax-based preference model, updating preferences using gradient ascent to maximize expected reward.

---