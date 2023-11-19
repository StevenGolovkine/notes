---
category: zettelkasten
tags:
  - "#topology"
  - "#sets"
creation date: 2023/11/15
Write article: false
Done article: false
---
# A set view of functions

Functions are characterised mathematical objects that create a correspondance (or mapping/transformation) between two sets. A function $f$ associates each element of $A$ to a unique element $f(x)$ in $B$. We associate to each function $f$ the set $\Gamma_f$ that contains all ordered pairs of the form $(x, f(x))$. The set $\Gamma_f$ is called the graph of $f$.

Some definitions, for a function $f: A \rightarrow B$, $X$ a subset of $A$ and $Y$ a subset of $B$:
- $f(X)$ is the image of $X$.
- $f^{-1}(Y)$ is the inverse image of $Y$.
- $A$ is the domain of $f$.
- $B$ is the range of $f$.

Injectivity (or one-one): $\forall x, y \in A, f(x) = f(y) \Rightarrow x = y$.
Surjectivity (or onto): $B = f(A)$.
Bijectivity = Injectivity + Surjectivity

Notations:
$$f(X) = \{f(x) \in B, \; x \in X\} = \{y \in B, \; \exists x \in X, y = f(x)\} \subset B$$
$$f^{-1}(Y) = \{x \in A, \; f(x) \in Y\} = \{x \in A, \; \exists y \in Y, x = f^{-1}(y)\} \subset A$$
