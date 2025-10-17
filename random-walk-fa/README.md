# 🧮 Random Walk with Function Approximation — Generalization in TD Learning

This subproject extends the **Random Walk** environment to study **function approximation** in reinforcement learning.  
Instead of maintaining separate value estimates for each discrete state, we approximate the value function using **parameterized models** (e.g., linear function approximation).  
This setup demonstrates how **Temporal Difference (TD)** learning behaves when the state space is large or continuous, where **generalization** and **approximation errors** become critical.

---

## 🧭 Overview

The **Random Walk** environment remains the same as in the tabular setting — a chain of states between two terminal ends, with the agent moving left or right randomly.  
However, rather than representing each state’s value explicitly, we use **feature vectors** to describe states and learn a **parameter vector θ** such that:

This formulation allows the agent to generalize value estimates across similar states — a fundamental step toward scaling RL to large or continuous domains.

---

## 🧠 Learning Objective

The learning update for **TD(0)** with linear function approximation is:

This captures the essence of **semi-gradient TD learning**, where the gradient is taken only with respect to the current state’s feature vector.

---

## ✅ What this project explores

- **TD(0) with linear function approximation**
- **n-step TD and TD(λ)** with parameterized value functions
- Comparison of **different feature representations**:
  - One-hot encoding (tabular baseline)
  - Coarse coding / tile coding
  - Polynomial or radial basis features
- Visualization of how generalization influences learning stability
- Empirical demonstrations of **divergence** under off-policy conditions

---
