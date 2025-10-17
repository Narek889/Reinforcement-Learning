# 🚶 Trajectory Sampling — Reinforcement Learning Experiments

This subproject explores **trajectory-sampling** methods in reinforcement learning: how to construct returns from sampled trajectories, how to use n-step and λ-style returns, and how to correct for off-policy data with importance sampling and its variance-reduced variants. The folder contains implementations, experimental harnesses, notebooks, and visualizations that illustrate bias/variance trade-offs, convergence behavior, and practical tips for using trajectory-based estimators in tabular and small-function-approximation settings.

---

## 📚 Why trajectory sampling matters

Trajectory sampling sits at the heart of model-free RL. Instead of relying on a full model of the environment, we estimate returns and update value/policy estimates from episodes (full trajectories) or from partial sequences (n-step trajectories). Trajectory-based estimators are central to Monte Carlo methods, n-step TD, and modern policy-gradient techniques that use advantage estimators and variance reduction. For off-policy problems, techniques such as importance sampling reweight observed trajectories so they provide unbiased (or asymptotically consistent) estimates for a target policy — but naive importance sampling often introduces high variance and needs careful handling. See foundational references for the theory behind many of these ideas. :contentReference[oaicite:0]{index=0}

---

## ✅ Highlights (what you’ll find here)

- Clear implementations of trajectory-based return estimators:
  - Full-episode Monte Carlo returns
  - n-step returns and TD(λ) style accumulation
  - Per-decision importance sampling & weighted importance sampling
- Experimental code to compare estimators on toy environments (gridworld, small MDPs)
- Notebooks with step-by-step visualizations of how returns and weights evolve
- Practical experiments showing bias vs variance trade-offs and how to stabilize off-policy estimates
- Scripts to reproduce results and save plots/logs for analysis

Key practical takeaway: trajectory sampling choices (n, λ, importance-sampling variant) greatly affect estimator variance and learning stability — and a few simple heuristics (weight clipping, normalization, weighted IS) make off-policy learning feasible in practice. :contentReference[oaicite:1]{index=1}

---
