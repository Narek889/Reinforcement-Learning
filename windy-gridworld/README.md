# 🌬️ Windy Gridworld – Reinforcement Learning with SARSA and Q-Learning

This project implements the classic Windy Gridworld environment from Sutton & Barto’s *Reinforcement Learning: An Introduction*. It explores two fundamental temporal-difference learning algorithms—SARSA and Q-Learning—to solve the navigation task in a stochastic environment influenced by wind.

---

## 📖 Overview

Windy Gridworld is a 7×10 grid where an agent must navigate from a start state to a goal state. Certain columns have a "wind" that pushes the agent upward, adding complexity to the pathfinding task. The objective is to learn an optimal policy that guides the agent to the goal in the fewest steps possible.

---

## 🧪 Environment Details

- **Grid Size**: 7 rows × 10 columns
- **Start State**: Typically at position (3, 0)
- **Goal State**: Typically at position (3, 7)
- **Actions**: Up, Down, Left, Right
- **Wind**: Columns 3 to 8 have upward wind of varying strength:
  - Columns 3, 4, 5: Wind strength 1
  - Columns 6, 7: Wind strength 2
  - Column 8: Wind strength 1
- **Rewards**:
  - Each step: -1
  - Reaching the goal: 0
- **Episode Termination**: Upon reaching the goal state

---

## 🧠 Implemented Algorithms

1. **SARSA (State-Action-Reward-State-Action)**:
   - On-policy TD control algorithm.
   - Updates action-value function based on the action actually taken.

2. **Q-Learning**:
   - Off-policy TD control algorithm.
   - Updates action-value function based on the maximum reward of the next state.

Both algorithms utilize an ε-greedy policy for action selection to balance exploration and exploitation.

---

## 📁 Repository Structure