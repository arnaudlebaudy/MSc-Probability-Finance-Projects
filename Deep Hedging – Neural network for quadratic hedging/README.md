This project implements a neural network approach to mean‑quadratic hedging for a European call option in a discrete‑time Black‑Scholes setting. The goal is to learn a hedging strategy that minimises the squared replication error. 

We compare the learned strategy to the analytical Black‑Scholes delta hedge. The network is a simple MLP one per time step. A two‑step training is used: pre‑training on the delta to stabilise initialisation, then fine‑tuning on the quadratic loss.

We also extend the model to include proportional transaction costs (\( f = 0.1\% \) per trade) and observe the impact on the hedging strategy and PnL distribution.

<img width="1789" height="789" alt="image" src="https://github.com/user-attachments/assets/4850ae15-ceff-4ba1-98b3-2c3c5fe7728e" />
<img width="989" height="490" alt="image" src="https://github.com/user-attachments/assets/e12a2490-68e0-4f83-b34d-a500af1f2b46" />


**References**  
- Buehler, H., Gonon, L., Teichmann, J., & Wood, B. (2019). *Deep hedging*. Quantitative Finance.  
