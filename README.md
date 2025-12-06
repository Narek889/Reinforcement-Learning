# ![Python](https://img.shields.io/badge/Python-3.8+-blue.svg) ![License](https://img.shields.io/badge/License-MIT-green.svg) ![Last Updated](https://img.shields.io/badge/Last%20Updated-2025--12--03-yellow.svg)

# 🤖 Reinforcement Learning

A comprehensive collection of Reinforcement Learning (RL) algorithm implementations based on Sutton and Barto's "Reinforcement Learning: An Introduction". This repository is intended as both a learning resource and a practical reference for core RL concepts and techniques.

---

## 📚 Overview

This repository contains well-documented Python implementations and experiments across many classic RL problems and methods. Each project is organized into its own directory and (where applicable) includes scripts or notebooks for experiments and visualization.

---

## 🗂️ Project Structure

Below are the project folders present in the repository based on the activity list you provided. If there are additional projects (you mentioned there should be 24 total), please paste the missing project names and I'll update this README accordingly.

- access-control
- blackjack
- cliff-walking
- coarse-coding
- counter-examples
- gambler-problem
- gridworld-dp
- gridworld-mdp
- infinite-variance
- maximization-bias
- mazes
- mountain-car-et
- mountain-car
- random-walk-et
- random-walk-fa
- random-walk-ntd
- random-walk
- ten-armed-testbed
- tic-tac-toe
- trajectory-sampling
- updates-comparison
- windy-gridworld

(If any of the above directories have been removed/renamed in the repo, tell me which ones to remove or rename.)

---

## 🧪 Implemented Algorithms & Topics

The repository covers implementations in the following areas:

- Multi-Armed Bandits (ε-greedy, UCB, optimistic initial values, gradient bandits)
- Monte Carlo methods (first-visit MC, exploring starts, on-policy & off-policy with importance sampling)
- Temporal-Difference learning (TD(0), n-step TD, SARSA, Q-Learning)
- Planning & model-based RL (Dyna-Q, Dyna-Q+, prioritized sweeping)
- Function approximation (state aggregation, coarse coding, tile coding/CMAC, polynomial & Fourier bases)
- Eligibility traces (TD(λ), SARSA(λ) with accumulating/replacing/Dutch traces)
- Average-reward methods (differential semi-gradient SARSA)
- Off-policy gradient-corrected algorithms (TDC / Expected TDC)
- Examples and counter-examples illustrating pitfalls (infinite variance, maximization bias, etc.)
- Classic environments and problems (mountain car, gridworlds, Blackjack, Tic-Tac-Toe, random walk variants, etc.)

---

## 🛠️ Requirements

- Python 3.x
- numpy
- matplotlib (for visualizations)
- tqdm (optional; progress bars)
- jupyter (optional; for notebooks)

Install common dependencies:

```bash
pip install numpy matplotlib tqdm jupyter
```

---

## 🚀 How to run experiments

Each project directory generally contains an entrypoint script or notebook:

Examples:
```bash
# Bandit experiments
cd ten-armed-testbed
jupyter notebook src_all/ten_armed_testbed.ipynb
# or
python src_all/ten_armed_testbed.py

# Tic-Tac-Toe
cd tic-tac-toe
python run_tic_tac_toe.py   # (if present) or open the README in that folder for exact usage

# Maze / Dyna-Q experiments
cd mazes
python run_dyna_maze.py      # (if present)

# Access control / differential SARSA
cd access-control
python run_access_control.py # (if present)
```

If a directory doesn't include a run script, open its README or the notebook files to learn how to reproduce experiments.

---

## 📁 Key modules (typical)

- Bandit implementations: ten-armed-testbed/src_all/bandit.py
- Tile coding utilities: mountain-car/src/tile_coding.py, access-control/src/tile_coding.py
- Maze / model classes: mazes/src/maze.py, mazes/src/models.py
- Blackjack implementation & Monte Carlo: blackjack/src/black_jack.py
- Tic-Tac-Toe state/player/judge: tic-tac-toe/src/state.py, tic-tac-toe/src/player.py, tic-tac-toe/src/judge.py
- Random walk examples & TD: random-walk-ntd, random-walk-et, random-walk-fa
- Function approximation utilities: coarse-coding/src/classes.py, coarse-coding/src/square_wave.py

---

## 📊 Sample Experiments

Highlights of experiments included in the repo:

- Ten-Armed Testbed: compare ε-greedy, UCB, optimistic initial values, and gradient bandit algorithms across many runs and steps.
- Mountain Car: tile coding feature representation with SARSA(λ) and different eligibility-trace schemes.
- Dyna Maze: Q-Learning with planning steps and prioritized sweeping comparisons.
- Random Walks: n-step TD vs. Monte Carlo vs. function approximation experiments.
- Access Control: differential semi-gradient SARSA for continuing tasks with average-reward learning.
- Counter-examples & Infinite variance: illustrate off-policy pitfalls and importance-sampling-related phenomena.

---

## 📖 Reference

This repository is heavily based on:

Sutton, R. S., & Barto, A. G. (2018). Reinforcement Learning: An Introduction (2nd ed.). MIT Press.  
http://incompleteideas.net/book/the-book-2nd.html

---

## 🤝 Contributing

Contributions are welcome! Please:
- Open issues for bugs or suggestions.
- Submit pull requests for improvements.
- Add README / usage examples within particular project directories.

---

## 👤 Author

**Narek889** — GitHub: https://github.com/Narek889

---
This README was last updated on December 6, 2025. 😊
