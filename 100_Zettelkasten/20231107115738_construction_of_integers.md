---
category: zettelkasten
tags:
  - topology
  - sets
creation date: 2023/11/07
Write article: false
Done article: false
---
# Construction of the set of integer

The set of integers $\mathbb{N}$ is a collection of objects on which a function $s$, the successor, has been defined such that the following conditions are true:
* $\forall x \in \mathbb{N}, \exists ! y \in \mathbb{N} \,/\, y = s(x)$, 
* $\forall x, y \in \mathbb{N}, s(x) = s(y) \Rightarrow x = y$
* There is one and only one object in $\mathbb{N}$ which is not the successor of an object in $\mathbb{N}$. This object is denoted $1$.
* Let $T \subset \mathbb{N} \,/\, 1 \in T$ and $\forall x \in T, s(x) \in T \Rightarrow T = \mathbb{N}$ (mathematical induction).

We define the sucessor function $s$ to be the addition, such that $s(x) = x + 1$. These conditions are the *Peano's axioms for the natural numbers*.