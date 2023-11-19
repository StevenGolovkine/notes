
---
creation date: 2023-03-28 11:21
last updated: 2023-03-28 11:21
---
# [[20230328112124_normalization_multivariate_functional_data]] - Normalization of multivariate functional data
__Tags__: #multivariate-functional-data 

---
__Contents__: Normalization can be done with the standard deviation of the curves at each sampling points ([[@chiouMultivariateFunctionalPrincipal2014]]).

Considering the set of multivariate curves $\{X^{(p)}(t)\}_{1 \leq p \leq P}$. Note $\mu^{(p)}(t) = \mathbb{E}(X^{(p)}(t))$, the point-wise mean curve of each components, and $v^{(p)}(t) = \texttt{Var}(X^{(p)}(t))$, the point-wise variance curve of each components.
The set of curves that are analysed are then
$$Z^{(p)}(t) = v^{(p)}(t)^{-1/2}\{X^{(p)}(t) - \mu^{(p)}(t)\}.$$

__References__:
[[@chiouMultivariateFunctionalPrincipal2014]] - Chiou, Chen and Yang - _Multivariate Functional Principal Component Analysis: A Normalization Approach_ (2014)