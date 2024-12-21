---
category: zettelkasten
tags: 
creation date: 2024/11/05
Write article: false
Done article: false
---
# First order stationary linear buffer

Study of the equation:
$$Dx = -\beta x, \quad\text{or}\quad L = D + \beta I$$
Link with linear regression: We regress change in $x$ ($Dx$) on $x$. The $\beta$ can be seen as regression coefficients (also named *rate function*).

Solution: 
$$x(t) = Ce^{-\beta t}, \quad C \neq 0$$
We can use any positive constant (different from $1$) to replace $e$, e.g. $10$ or $2$. The solution exhibits exponential decay when $\beta >0$ and exponential growth when $\beta < 0$.

Corresponding operator equation: $Lx = \beta x + Dx = 0$. The solution space of the equation is the *kernel* of $L$.

