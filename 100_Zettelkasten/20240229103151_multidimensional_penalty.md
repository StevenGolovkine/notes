---
category: zettelkasten
tags:
  - splines
creation date: 2024/02/29
Write article: false
Done article: false
---
# Multidimensional penalty

Penalty are indispensable in multiple dimension, because all basis functions need to be well supported by the data locations.

Let $A$ be the matrix of coefficients to be estimated. Let $D^{(1)}$ and $D^{(2)}$ be the matrices that performed the "difference" operator on the rows and the columns. The penalty is construct as
$$\text{Penalty} = \lambda^{(1)}\lvert\!\lvert D^{(1)}A\rvert\!\rvert_F^2 + \lambda^{(2)}\lvert\!\lvert D^{(2)}A\rvert\!\rvert_F^2.$$
The two lambdas allow anisotropic smoothing according to the first of second dimension.
As we work with $\text{vec}(A) = \alpha$, the penalty needs to be rewritten using Kronecker products
$$\text{Penalty} = \lambda^{(1)}\lvert\!\lvert (I^{(2)} \otimes D^{(1)})\alpha\rvert\!\rvert^2 + \lambda^{(2)}\lvert\!\lvert (D^{(2)} \otimes I^{(1)})\alpha\rvert\!\rvert_F^2 = \lambda^{(1)} \alpha^\top P^{(1)}\alpha + \lambda^{(2)}\alpha^\top P^{(2)}\alpha,$$
where $P^{(1)} = (I^{(2)} \otimes D^{(1)})^\top(I^{(2)} \otimes D^{(1)})$ and $P^{(2)} = (D^{(2)} \otimes I^{(1)})^\top(D^{(2)} \otimes I^{(1)})$.

Note that as the coefficients remain on a grid, the penalty does not depend on whether the data are scattered or on a grid because in either case, there is the full coefficient matrix $A$.

Finally, the minimizer of the objective function is given by
$$\widehat{\alpha} = \left(B^\top\text{diag}(w) B + \lambda^{(1)}P^{(1)} + \lambda^{(2)}P^{(2)}\right)^{-1}B^\top \text{diag}(w)y.$$


