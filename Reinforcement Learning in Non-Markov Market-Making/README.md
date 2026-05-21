This project implements the paper *Reinforcement Learning in Non‑Markov Market Making* by J. Lalor & A. Swishchuk (2024) – a deep reinforcement learning approach to optimal market making where the mid‑price follows Hawkes or semi‑Markov processes instead of the usual Markovian diffusion.

We formulate market making as an MDP, train a Soft Actor‑Critic agent on a discrete action space (buy/hold/sell). The agent learns to manage inventory risk while capturing realistic limit‑order‑book features. Our implementation reproduces the main results of the paper, showing improved reward over the baseline, although hyperparameter sensitivity remains a challenge.

**Reference:** Lalor, J. & Swishchuk, A. (2024). *Reinforcement learning in non‑Markov market making*. arXiv:2410.14504 / Risks 13(3):40 (2025).

The source code is available upon request.
