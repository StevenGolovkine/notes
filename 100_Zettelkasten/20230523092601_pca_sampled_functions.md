
---
creation date: 2023-05-23 09:26
last updated: 2023-05-23 09:26
---
# [[20230523092601_pca_sampled_functions]] - PCA of sampled functions
__Tags__: #functional-principal-components  #reproducing-kernel-hilbert-space 

---
__Contents__: Incorporating information on curve derivatives in FPCA can be done by a change of metric in the row space. A RKHS defines the best interpolating functions ([[20230523093049_rkhs]]).


Let $H^m(T)$ the space of $m - 1$ absolutely continuous derivatives on $T$. Let the function $x \in H^m(T)$ such that
$$x: t \rightarrow u(t) + e(t).$$
We assume that
* The function $u$ satifies a linear differential equation
$$Lu(t) = \sum_{j=1}^m a_j \frac{d^j u}{dt^j}(t) = 0.$$ The function $u$ is in $H_1$ where $H_1$ is the space of functions within $H^m(T)$ that satisfies the linear differential equation.
* The function $e$ is in $H^m(T)$ but not in H_1, denoted by $H_2$.
* $H^m(T) = H_1 \oplus H_2$

We define different inner-product for each of the spaces:
* For $H_2$, $\langle x, y \rangle_2 = \int Lx(t)Ly(t)dt$, use the linear differential equation
* For $H_1$, $\langle x, y \rangle_1 = \sum_{j=1}^m B_j(x)B_j(y)$, use the boundary conditions
* For $H^m$, $\langle x, y \rangle_0 = \langle x, y \rangle_1 + \langle x, y \rangle_2$.
The FPCA can then be done in $H^m(T)$, $H_1$ or $H_2$.

The FPCA of the interpolated functions is equivalent to the classical PCA of sampled values in a particular metric.


__References__:
[[@bessePrincipalComponentsAnalysis1986]] - Besse and Ramsay - _Principal components analysis of sampled functions_ (1986)

