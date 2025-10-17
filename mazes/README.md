# 🗺️ Mazes — Reinforcement Learning Environments & Experiments

This subproject contains maze environments, agents, and experiments designed to study navigation, exploration, planning vs. learning, and representation in reinforcement learning. It includes a collection of handcrafted mazes (gridworlds with walls, doors, keys, rewards), environment wrappers, baseline agents (tabular and function-approx), and notebooks/scripts to run systematic experiments and visualize trajectories, learned value/policy maps, and exploration behavior.

---

## 🧭 Project goals

- Provide a diverse set of maze environments for testing navigation and exploration algorithms (sparse rewards, dead-ends, long corridors, multi-room layouts).
- Compare learning algorithms and exploration strategies (e.g., ε-greedy, Boltzmann, count-based bonuses, intrinsic motivation).
- Demonstrate planning vs model-free learning by including model-based baselines (value iteration / Dijkstra) where applicable.
- Offer tools for visualization (trajectory overlay, heatmaps of state visitation, value-function and policy plots) to diagnose learning and exploration failure modes.

---

## ✅ Highlights (what’s included)

- Multiple maze maps of varying complexity (small toy mazes → large multi-room mazes).
- Gridworld environment implementation with support for:
  - Deterministic and stochastic transitions
  - Walls, doors, keys (simple inventory), and teleporters
  - Sparse terminal rewards, shaped rewards, and per-step penalties
- Agent implementations:
  - Tabular Q-Learning and SARSA
  - n-step and TD(λ) variants
  - Epsilon-greedy, Boltzmann, and simple intrinsic-reward explorers (count-based / pseudo-counts)
  - Model-based planner: value iteration / BFS path planner for comparison
  - Optional function-approx agents (linear features / small NN)
- Experiment harnesses and notebooks to run parameter sweeps, seed averaging, and produce publication-quality plots.
- Visualization utilities:
  - Maze renderers with trajectory overlays
  - State visitation heatmaps (log-scaled)
  - Animated episode playback (GIF / inline notebook animation)

---
