---
category: zettelkasten
tags:
  - "#inequality"
creation date: 2024/01/17
Write article: false
Done article: false
---
# Cauchy Schwarz inequality

Let $x = (x_1, \dots, x_n)$ and $y = (y_1, \dots, y_n)$ be vectors of $\mathbb{R}^n$.
$$\langle x, y \rangle \leq \lvert\vert x \rvert\rvert \cdot \lvert \lvert y \rvert\rvert$$

**Proof**
To prove the inequality, we are going to prove the square of it.
Consider, for $\lambda \in \mathbb{R}$, the expression $\sum_{i = 1}^n (x_i + \lambda y_i)^2$. We have
$$0 \leq \sum_{i = 1}^n (x_i + \lambda y_i)^2 = \sum_{i = 1}^n x_i^2 + 2\lambda \sum_{i = 1}^nx_iy_i + \lambda^2\sum_{i = 1}^n y_i^2 = \lvert\lvert x \rvert\rvert^2 + 2\lambda\langle x, y \rangle + \lambda^2\lvert\lvert y \rvert\rvert^2.$$

Therefore, the quadratic equation in $\lambda$, $\lvert\lvert x \rvert\rvert^2 + 2\lambda\langle x, y \rangle + \lambda^2\lvert\lvert y \rvert\rvert^2 = 0$, can have at most one real solution.
Consequently, $\Delta < 0$ and finally
$$\langle x, y \rangle^2 - \lvert\lvert x \rvert\rvert^2 \cdot \lvert\lvert y \rvert\rvert^2 \leq 0$$


This inequality can be extended to elements of an Hilbert space $H$ (the proof is given by bounding the partial sums of the serie of positive terms).

A similar inequality is given by
$$\lvert\lvert x + y \rvert\rvert \leq \lvert\lvert x \rvert\rvert + \lvert\lvert y \rvert\rvert.$$
The proof is straighforward reamrking that if $x, y \in \mathbb{R}^n$ (resp. $H$), $x + y \in \mathbb{R}^n$ (resp. $H$).