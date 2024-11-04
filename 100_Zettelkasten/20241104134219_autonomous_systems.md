---
category: zettelkasten
tags:
  - "#dynamics"
creation date: 2024/11/04
Write article: false
Done article: false
---
# Autonomous systems

Autonomous systems are dynamical systems without input variables. General notation: $Dx = f(x | \theta)$.

Example of polynomials:
$$D^m x(t) = 0 \Longrightarrow x(t) = \sum_{i = 0}^{m - 1} a_it^i$$
Example of first order buffer:
$$Dx = -\beta x \Longrightarrow x(t) = C\exp(-\beta t)$$
Example of second order buffer:
$$ D^2 x = -\beta_0x - \beta_1 Dx$$
