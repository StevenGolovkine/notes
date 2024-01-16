---
category: zettelkasten
tags:
  - topology
creation date: 2024/01/15
Write article: false
Done article: false
---
# Topological equivalence

Two metric spaces $(A, d_A)$ and $(B, d_B)$ are topologically equivalent if there are inverse functions $f: A \rightarrow B$ and $g: B \rightarrow A$ such that $f$ and $g$ are continuous.

**Sufficient condition for the topological equivalence of two metric spaces with the same underlying set**
Let $(X, d_1)$ and $(X, d_2)$ be two metric spaces.
If $\exists K > 0 / \forall x, y \in X, d_2(x, y) \leq K d_1(x, y)$, then the identity mapping $i: (X, d_1) \rightarrow (X, d_2)$ is continuous.
If $\exists K_1, K_2 > 0 / \forall x, y \in X, d_2(x, y) \leq K_1 d_1(x, y)$ and $d_1(x, y) \leq K_2 d_2(x, y)$, then the identity mappings define a topological equivalence between $(X, d_1)$ and $(X, d_2)$.

**Examples**: The metric space $(\mathbb{R}^n, d_1)$ and $(\mathbb{R}^n, d_2)$ where $d_1(x, y) = \max_i \lvert x_i - y_i \rvert$ and $d_2(x, y) = \sqrt{\sum_i (x_i - y_i)^2}$, are topologically equivalent.

**Sufficient condition for the topological equivalence of two metric spaces**:
Let $(X, d_1)$ and $(Y, d_2)$ be two metric spaces. Let $f: X \rightarrow Y$ and $g: Y \rightarrow X$ be inverse functions. Then, the following statements are equivalent:
1. $f$ and $g$ are continuous.
2. A subset $O$ of $X$ is open $\Leftrightarrow$ $f(O)$ is an open subset of $Y$.
3. A subset $F$ of $X$ is closed $\Leftrightarrow$ $f(F)$ is a closed subset of $Y$.
4. For each $x \in X$, for each subset $N$ of $X$, $N$ is a neighborhood of $x$ $\Leftrightarrow$ $f(N)$ is a neighborhood of $f(x)$.