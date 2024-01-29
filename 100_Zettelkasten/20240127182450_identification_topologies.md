---
category: zettelkasten
tags:
  - topological-space
creation date: 2024/01/27
Write article: false
Done article: false
---
# Identification topologies

Let $(A, \mathfrak{S})$ and $(B, \mathfrak{S}^\prime)$ be topological spaces. Let $p: (A, \mathfrak{S}) \rightarrow (B, \mathfrak{S}^\prime)$ be a continuous function mapping $(A, \mathfrak{S})$ onto $(B, \mathfrak{S}^\prime)$.

The function $p$ is an identification if $\forall U \subset B, p^{-1}(U)$ is open in $A \Rightarrow U$ is open in $B$.

Let $Y$ is a set (without a topology) and let $G: A \rightarrow Y$ be a continous function such that for each $x, x^\prime \in A$ with $p(x) = p(x^\prime)$, we also have $G(x) = G(x^\prime)$. Then, for each $b \in B$, we may choose any $x \in p^{-1}(\{b\}) \subset A$, define $g(b) = G(x)$ and the resulting funtion $g$ is continuous

Let $p: (X, \mathfrak{S}) \rightarrow Y$. The identification topology on $Y$ determined by $p$ consists of those sets $U \subset Y$ such that $p^{-1}(U)$ is open in $X$.