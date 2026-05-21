This project implements the mathematical model of Uniswap V3. We simulate a liquidity pool with multiple price ticks, a CEX price following geometric Brownian motion, and a swap mechanism that triggers whenever the Automated Market Makers price deviates beyond the fee band, restoring the no‑arbitrage condition.

We track real reserves per tick, fees collected in both tokens, and total position value over time. The simulation reproduces key theoretical results: the trade‑off between fee rate and swap frequency, the asymptotic convergence of fees as the fee rate tends to zero, and the effect of CEX price sampling frequency on detected swaps.

<img width="1589" height="790" alt="traj2" src="https://github.com/user-attachments/assets/372184d2-3797-4648-9f84-27d9a4f382ac" />

**References:**  
- Angeris, G., Kao, H.T., Chiang, R., Noyes, C. & Chitra, T. (2021). *An analysis of Uniswap markets*.  
- Echenim, M., Gobet, E. & Maurice, A.C. (2025). *Uniswap v3: Impermanent Loss Modeling and Swap Fees Asymptotic Analysis*.

The source code is available upon request.
