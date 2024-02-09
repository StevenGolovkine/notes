---
category: zettelkasten
tags:
  - connectedness
creation date: 2024/02/09
Write article: false
Done article: false
---
# Path connectedness

Let $(X, \mathfrak{S})$, $(Y, \mathfrak{S}^\prime)$ be topological spaces. 

A continuous function $f: [0, 1] \rightarrow X$ is called a path in $X$.
The path $f$ is said to connect (or join) the point $f(0)$ to the point $f(1)$, $f(0)$ is called the initial point and $f(1)$ is called the terminal point of the path $f$. If $f(0) = f(1)$, the path is a closed path (or a loop).
If $f$ is a path in $X$, $f([0, 1])$ is called a curve in $X$.

$(X, \mathfrak{S})$ is said to be path-connected if, for each pair of points $u, v \in X$, there is a path $f$ connecting $u$ to $v$.

**Examples**:
- The real line $\mathbb{R}$ is path-connected. For if $a, b$ two real numbers, the path $f: [0, 1] \rightarrow \mathbb{R}$ defined by $f(t) = a + (b - a)t$ for $t \in [0, 1]$ connects $f(0) = a$ and $f(1) = b$.
- $\mathbb{R}^n$ is path-connected.
- $S^n$ is path-connected.

**Properties**:
- If $(X, \mathfrak{S})$ is path-connected and it exists a continuous mapping $g: X \rightarrow Y$, which is onto, then $(Y, \mathfrak{S}^\prime)$ is path-connected.

**Path connectedness $\Longrightarrow$ connectedness** (but the converse is false)
