---
category: zettelkasten
tags:
  - "#dynamics"
  - "#differential-equation"
creation date: 2024/11/04
Write article: false
Done article: false
---
# Linear differential equations

The linearity in differential equations refers of the linearity of the function $f$ with respect to its arguments $x$ and its derivatives.

Example of order $m$ buffer:
$$D^m x = \sum_{j = 0}^{m - 1}\beta_j D^j x$$
The coefficients $\beta_j$ may vary over $t$ but must not depend on $x$. When all the coefficients are constants, the system is *stationary*.

A general version of linear differential equations is given by:
$$D^m x(t) = \sum_{j = 0}^{m - 1}b_j\beta_j(t | \theta) D^j x(t) + \sum_{l = 0}^L a_l\alpha_l(t)u_l(t), m > 0,$$
where $u$ is a *forcing* function, the rate function $\beta_j$ can vary over time (and determined by the parameter vector $\theta$, some estimated from the data) but not be a function of $x$ and a known constant $b$ ($1$ or $-1$).

Example of first order stationary linear buffer ([[20241105133025_first_order_stationary_linear_buffer]]).
Example of second order stationary linear buffer ([[20241105141554_second_order_stationary_linear_equation]]).
