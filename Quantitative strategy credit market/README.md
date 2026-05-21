This project follows the methodology of Laloux et al. (1999, 2000) to distinguish signal from noise in empirical correlation matrices, first on S&P 500 stock returns, then on a dataset of CDS spreads.

We compute the empirical correlation matrix from weekly returns (or spread changes), compare its eigenvalue distribution to the Marchenko‑Pastur law (the null hypothesis of pure noise), and filter out the noisy eigenvalues. Only the eigenvalues above the theoretical upper bound are kept as informative. The rest are replaced by a constant that preserves the trace of the matrix.

We then build efficient frontiers using both the raw and the filtered covariance matrices, and compare the predicted risk (in‑sample) to the realised risk (out‑of‑sample).

<table>
  <tr>
    <td><img width="100%" src="https://github.com/user-attachments/assets/6113982b-c4df-4a98-b798-7216870f26ab" /></td>
    <td><img width="100%" src="https://github.com/user-attachments/assets/e5658115-16a4-4988-b867-cf5a48925233" /></td>
  </tr>
</table>

**Reference:** Laloux, L., Cizeau, P., Potters, M. & Bouchaud, J.P. (1999–2000). Random matrix theory and financial correlations.
