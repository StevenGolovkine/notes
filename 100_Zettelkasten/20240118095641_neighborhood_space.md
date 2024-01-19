---
category: zettelkasten
tags:
  - neighborhood-space
creation date: 2024/01/18
Write article: false
Done article: false
---
# Neighborhood space

Let $X$ be a set and for each point $x \in X$, let $\mathfrak{N}_x$ be a collection of subsets of $X$ (called the neighborhoods of $x$) satisfying the properties:
- For each $x \in X$, it exists at least one neightborhood of $x$.
- For each $x \in X$ and each neighborhood $N$ of $x$, $x \in N$.
- For each $x \in X$, if $N$ is a neighborhood of $x$ and $N \subset N^\prime$, then $N^\prime$ is a neighborhood of $x$.
- For each $x \in X$ and each pair $(N, M)$ of neighborhood of $x$, $N \cap M$ is a neighborhood of $x$.
- For each $x \in X$ and each neighborhood $N$ of $x$, there exists a neighborhood $O$ of $x$ such that $O \subset N$ and $O$ is a neighborhood of each of its points.

The object $(X, \mathfrak{N})$ is a neighborhood space.

**Pay attention**: In the definition of a neighborhood space, the notion of open set is not defined. So, the term *open set* is meaningless in a neighborhood space until we defined it.