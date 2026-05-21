This project implements the theoretical framework of Bonesini et al. (2023) for simulating non‑Markovian stochastic Volterra processes. We focus on the fractional kernel case (rough volatility), where a non‑Markovian "elephant" process X is transformed into a Markovian goldfish process xi. An Euler scheme is applied to xi, then used to reconstruct X via a pseudo‑integrated scheme that handles the singular kernel correctly.

We compare two factorisation methods (LDL and SVD) for generating the correlated Gaussian vectors required by the scheme. The simulation reproduces the burst of memory phenomenon when the initial condition is non‑zero, and confirms the theoretical convergence of E[xi_t] and E[X_t] to their limits. The strong convergence study shows an error rate close to 1/2 when the diffusion term dominates, independent of the Hurst parameter – a key advantage over direct discretisations of Volterra equations.

<table>
  <tr>
    <td><img width="100%" src="https://github.com/user-attachments/assets/0e7abfa6-bee5-4d37-95d9-91990a22a00d" /></td>
    <td><img width="100%" src="https://github.com/user-attachments/assets/b71c4cf2-8bfe-4994-b2b2-533971feed6a" /></td>
    <td><img width="100%" src="https://github.com/user-attachments/assets/202416fd-72b4-4c0d-b0b8-cbc76f5dbde2" /></td>
  </tr>
</table>

**Reference:** Bonesini, O., Callegaro, G., Grasselli, M. & Pagès, G. (2023). *From elephant to goldfish (and back): memory in stochastic Volterra processes*.

The report and source code can be provided upon request.
