# 🎰 Gambler's Problem – Dynamic Programming in Reinforcement Learning

This project provides an implementation of the classic **Gambler's Problem** using dynamic programming techniques, specifically **Value Iteration** and **Policy Iteration**, as introduced in Sutton & Barto's *Reinforcement Learning: An Introduction* (Chapter 4, Example 4.3).

---

## 📖 Problem Description

The Gambler's Problem is a finite, episodic Markov Decision Process (MDP) defined as follows:

- **States**: The gambler's capital, ranging from \$0 to \$100.
- **Actions**: At each state, the gambler can bet any amount up to the minimum of their current capital and the difference between their capital and \$100.
- **Transitions**:
  - With probability *p*, the gambler wins the bet and increases their capital by the bet amount.
  - With probability *(1 - p)*, the gambler loses the bet and decreases their capital by the bet amount.
- **Rewards**:
  - A reward of 0 for all transitions, except when reaching the goal state (\$100), which yields a reward of 1.
- **Terminal States**: \$0 (bankruptcy) and \$100 (goal).

The objective is to determine the optimal policy that maximizes the probability of reaching the goal state from each starting capital.

---

## 🧠 Implemented Algorithms

- **Value Iteration**: Iteratively updates the value function for each state until convergence, then derives the optimal policy.
- **Policy Iteration**: Alternates between policy evaluation and policy improvement steps until the policy stabilizes.

These algorithms are implemented in the `src/` directory.

---