---
category: zettelkasten
tags:
  - "#topology"
  - "#sets"
creation date: 2023/11/18
Write article: false
Done article: false
---
# Mathematical relations using sets

A relation is an extension of a function.

A relation $R$ from the elements of a set $A$ to the elements of a set $B$ is as subset of $A \times B$. Given $a \in A$ and $b \in B$, we write the relation between $a$ and $b$ as $a R b$.

Properties of a relation $R$ of a set $E$:
- reflexive: $a R a$ for all $a \in E$.
- symmetric: $a R b$ $\Longleftrightarrow$ $b R a$.
- transitive: $a R b$ and $b R c$ $\Longrightarrow$ $a R c$.
- equivalent: reflexive + symmetric + transitive

Equivalent class: Let $R$ be a relation class on a set $E$. For each $a \in E$, we note $\pi(a)$ the equivalence class of $a$. It is the subset of $E$ with all its element $x$ such that $a R x$:
$$\pi(a) = \{x \in E, \; a R x\}.$$
Two equivalence classes are either disjoint or identical. Let $\pi(a)$ and $\pi(a^\prime)$, two equivalence classes. If it exists $x \in E$ such that $x \in \pi(a)$ and $x \in \pi(a^\prime)$, then $\pi(a) = \pi(a^\prime)$.