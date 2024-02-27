---
category: zettelkasten
tags:
  - splines
creation date: 2024/02/27
Write article: false
Done article: false
---
# Derivatives of P-splines

Assuming that the set of coefficient $\alpha$ has been estimated. Derivatives of oder $k$ can be computed using
$$\frac{d^k}{dt^k} \sum_{j}B_j(t, p)\alpha_j = \sum_{j} \frac{\Delta^k \alpha_j}{h^k}B_j(t, p-k).$$
A necessary condition is that $p > k$ (degree of the B-splines greater than the derivative degree), otherwise the B-splines of degree $p - k$ will be zero everywhere.

When $\widehat{y} = B\widehat{\alpha}$, we get
$$\frac{d^k}{dt^k}\widehat{\mu} = \frac{\widetilde{B}(D_k\widehat{\alpha})}{h^k}.$$



