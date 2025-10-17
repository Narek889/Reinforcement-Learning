# 🤖 Reinforcement Learning Projects

Welcome to my collection of Reinforcement Learning (RL) projects! This repository features practical implementations of core RL algorithms inspired by Sutton & Barto’s classic book *Reinforcement Learning: An Introduction*. Each sub-project is designed to illustrate key RL concepts using simple environments.

---

## 📁 Projects Overview

| Project | Description | Algorithms |
|--------|-------------|------------|
| [🃏 Blackjack](./blackjack) | Train an agent to play simplified Blackjack using Gym. | Q-Learning, Deep Q-Network (DQN) |
| [🚶‍♂️ Random Walk](./random-walk) | Estimate value functions in a linear environment. | Monte Carlo, TD(0), n-step TD, TD(λ) |
| [🚶 Random Walk — n-step TD](./random-walk-ntd) | Study n-step TD methods on Random Walk, comparing bias, variance, and convergence. | n-step TD, Monte Carlo |
| [🚶 Random Walk — Function Approximation](./random-walk-fa) | Apply linear function approximation to Random Walk. | TD(0), n-step TD, TD(λ) with linear FA |
| [🎨 Coarse Coding](./coarse-coding) | Feature-based generalization using overlapping tiles. | TD(0), n-step TD, TD(λ) with coarse-coded features |
| [🎲 Trajectory Sampling](./trajectory-sampling) | Construct returns from sampled trajectories and correct off-policy data. | n-step returns, λ-returns, Importance Sampling |
| [🌬️ Windy Gridworld](./windy-gridworld) | Navigate a grid under stochastic wind forces. | SARSA, Q-Learning, Expected SARSA |
| [🗺️ Mazes](./mazes) | Tabular and function approximation agents navigating complex mazes. | Q-Learning, SARSA, n-step TD, Planning (Value Iteration/A*) |
| [📊 Updates Comparison](./updates-comparison) | Compare TD update methods for bias, variance, and convergence. | TD(0), n-step TD, TD(λ), Monte Carlo |
| [🎰 Gambler's Problem](./gambler-problem) | Optimal betting strategy problem. | Dynamic Programming |
| [🗺️ Gridworld (DP)](./gridworld-dp) | Solve Gridworld using full model knowledge. | Value Iteration, Policy Iteration |
| [📊 Gridworld (MDP)](./gridworld-mdp) | Model Gridworld as an MDP. | MDP Framework, Bellman Updates |
| [🎯 10-Armed Testbed](./ten-armed-testbed) | Explore action selection strategies in a multi-armed bandit setup. | ε-greedy, UCB, Optimistic Init |
| [❌⭕ Tic-Tac-Toe](./tic-tac-toe) | Learn to play Tic-Tac-Toe through self-play. | Tabular Value Function |
| [🌄 Cliff Walking](./cliff-walking) | Navigate a cliff-edge environment. | SARSA, Q-Learning |
| [♾️ Infinite Variance](./infinite-variance) | Explore scenarios leading to infinite variance in Monte Carlo estimates. | Monte Carlo Methods |
| [🎲 Maximization Bias](./maximization-bias) | Demonstrate the effect of maximization bias in value estimation. | Q-Learning, SARSA |

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/Narek889/Reinforcement-Learning.git
cd Reinforcement-Learning
