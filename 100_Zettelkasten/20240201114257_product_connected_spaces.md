---
category: zettelkasten
tags:
  - connectedness
  - topological-space
creation date: 2024/02/01
Write article: false
Done article: false
---
# Product of connected topological spaces

Let $(X, \mathfrak{S})$ and $(Y, \mathfrak{S}^\prime)$ be connected topological spaces. Then $X \times Y$ is connected.

Let $(X_1, \mathfrak{S}_1), \dots, (X_n, \mathfrak{S}_n)$ be connected topological spaces. Then $\prod_{i = 1}^n X_i$ is a connected topological space.

Let $\{(X_\alpha, \mathfrak{S}_\alpha)\}_{\alpha \in I}$ be an indexed family of topological spaces each of which is connected. Let $x$ and $x^\prime$ be two points of $X = \prod_{\alpha \in I} X_\alpha$ such that $x(\alpha) = x^\prime(\alpha)$ except on a finite set of indices $I^\prime \subset I$ and let $f: X \rightarrow \{0, 1\}$ be continuous. Then $f(x) = f(x^\prime)$.
$X = \prod_{\alpha \in I} X_\alpha$ is connected if each $X_\alpha$ is connected.