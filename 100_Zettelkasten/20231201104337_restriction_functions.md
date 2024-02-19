---
category: zettelkasten
tags:
  - "#sets"
  - topology
creation date: 2023/12/01
Write article: false
Done article: false
---
# Restriction and extension of functions

The restriction and extension of a function is a particular case of compositions. It consists of a composition with the identity function defined on particular domains.

Let $X \subset A$ and define two functions $f: X \rightarrow Y$ and $g: A \rightarrow Y$. If for each $x \in X$, $f(x) = g(x)$, then $f$ is a restriction of $g$ to $X$ and $g$ is an extension of $f$ to $A$.
We note $f = \left.g\right|_X$.

Define the identity function: $i: X \rightarrow A$ such that $i(x) = x$. The restriction is 
$$\forall x \in X, f(x) = g \circ i (x).$$
![[restriction_figure_1.png|200]]

The diagram is thus commutative.


**Definition in topological space:**
Let $(X, \mathfrak{S})$ be a topological space and let $A, B$ be closed subsets of this space. Let $g: A \rightarrow Y$ and $h: B \rightarrow Y$ be continuous functions with the property that for $x \in A \cap B, g(x) = h(x)$. Then the function $k: A \cup B \rightarrow Y$ defined by $k(x) = g(x), x \in A$ and $k(x) = h(x), x \in B$ is a continuous extension of $g$ and $h$.