---
category: zettelkasten
tags:
  - sets
creation date: 2024/02/07
Write article: false
Done article: false
---
# Antipodal points

If $x = (x_1, \dots, x_{n+1}) \in S^n$. The points $(-x_1, \dots, -x_{n+1})$, denoted by $-x$, is called the antipodal point of $x$.

Consider a continuous function $f: S^1 \rightarrow \mathbb{R}$. Define the function $F: S^1 \rightarrow \mathbb{R}$ by $F(x) = f(x) - f(-x)$.
For some $z \in S^1$, $F(z) = 0$ that is $f(z) = f(-z)$.

Borsuk-Ulam theorem:
Let $f: S^n \rightarrow \mathbb{R}^n$ be continuous. Then there exists a pair of antipodal points $z, -z \in S^n$ such that $f(z) = f(-z)$.

