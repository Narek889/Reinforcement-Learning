# 🎲 Random Walk — n-step TD Experiments

This subproject implements and compares **n-step Temporal Difference (n-step TD)** learning on the classic **Random Walk** problem — a simple, controlled environment that demonstrates the relationship between Monte Carlo (infinite-step) and one-step TD learning. It provides clean code, experiments, and visualizations to illustrate how the number of backup steps `n` affects **bias**, **variance**, and **learning speed**.

---

## 🧭 Overview

The **Random Walk** task is a benchmark from Sutton & Barto’s *Reinforcement Learning: An Introduction*.  
An agent starts in the middle of a 1D chain of states and moves left or right randomly until it reaches a terminal state. Rewards occur only at the terminal ends (typically +1 on the right, 0 on the left).  

This setup is simple yet powerful — it allows clear, quantitative comparisons of TD learning methods and how multi-step targets influence convergence and stability.

---

## ✅ What this project explores

- Implementation of **n-step TD** learning (for any `n ≥ 1`)
- Empirical comparison of **TD(0)**, **n-step TD**, and **Monte Carlo** (infinite-step) targets  
- Study of **bias vs variance** trade-offs as a function of `n`
- Sensitivity to **learning rate (α)** and **discount factor (γ)**
- Aggregated results across random seeds for statistical reliability

---
