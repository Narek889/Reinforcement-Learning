# 🎨 Coarse Coding — Function Approximation in Reinforcement Learning

This subproject demonstrates **coarse coding** as a feature representation method for reinforcement learning.  
Instead of using one-hot state representations, states are mapped to **overlapping receptive fields (tiles)** to allow **generalization across similar states**.  
The experiments include tabular agents with coarse-coded features, n-step TD learning, and visualizations showing how feature overlap affects learning speed, bias, and stability.

---

## 🧭 Overview

**Coarse coding** partitions the state space into multiple overlapping regions, or tiles.  
Each tile corresponds to a binary feature (active/inactive), and a single state can activate multiple features simultaneously.  

This representation enables **linear function approximation** in RL:

- Value function estimate: `v_hat(s; theta) = sum_i theta[i] * x_i(s)`, where `x_i(s)` is 1 if tile i is active for state s.
- Each weight `theta[i]` is updated using TD rules.

Benefits:

- Generalization across states improves sample efficiency.
- Smooths learning curves compared to tabular representations.
- Helps visualize the effect of overlapping features on convergence and bias.

---

## ✅ Highlights

- Implementation of coarse-coded feature vectors for 1D and 2D state spaces.
- TD(0), n-step TD, and TD(λ) with coarse-coded features.
- Parameter sweeps for:
  - Number of tilings
  - Tile width
  - Learning rate (α)
  - Discount factor (γ)
- Visualization of feature activations, state-value approximation, and learning trajectories.
- Experimental notebooks for reproducibility and analysis.

---
