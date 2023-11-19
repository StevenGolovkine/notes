
---
creation date: 2023-03-27 16:08
last updated: 2023-03-27 16:08
---
# [[20230327160843_karhunen_loeve_expansion]] - Karhunen-Loève expansion
__Tags__: #functional-data #dimension-reduction 

---
__Contents__: Curves can be expanded in a particular set of basis function.

$$X(t) = \mu(t) + \sum_{k = 1}^{\infty} c_k\psi_k(t), \quad t \in \mathcal{T},$$
where 
* the coefficients $c_k$ are the projection of the curves onto the eigenfunctions.
* the functions $\psi_k$ are the eigenfunctions.
This is refered as the Karhunen-Loève expansion. The coefficients $c_k$ are centered and $\text{Cov}(c_k, c_l) = \lambda_k \delta_{kl}$, with $\lambda_k$ are the eigenvalues. The eigenvalues converge to $0$ as $k$ goes to $\infty$. This representation is valid for both univariate and multivariate functional data.

In practice, we use a truncated version of the KL expansion.

__References__:



