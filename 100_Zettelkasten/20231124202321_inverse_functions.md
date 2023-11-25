---
category: zettelkasten
tags:
  - "#topology"
  - sets
creation date: 2023/11/24
Write article: false
Done article: false
---
# Inverse of functions

The inverse of a function is a a particulat case of composition. Let $f: A \rightarrow B$ and $g: B \rightarrow A$ be two functions. We say that $g$ is the inverse of $f$, if for all $x \in A$, $g(f(x)) = x$ and $f$ is the inverse of $g$, if for all $x \in B$, $f(g(x)) = x$.

![[inverse_figure_1.png|200]]

Theorems:
1. If two functions are inverse of one another, then they are bijectives.
2. If a function is bijective, then the function is invertible.
3. If a function is invertible, then the inverse is unique.

These theorems can be summarised in the following way:

Given $f: A \rightarrow B$, a necessary and sufficient condition, that there exists a unique function $g: B \rightarrow A$ such that these two functions are inverse functions, is that $f: A \rightarrow B$ be one-one and onto.