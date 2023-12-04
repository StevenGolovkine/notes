---
category: zettelkasten
tags:
  - sets
  - topology
creation date: 2023/12/04
Write article: false
Done article: false
---
# Arbitrary products of sets

Let $\{X_\alpha\}_{\alpha \in I}$ be an indexed family of sets. We note $\prod_{\alpha \in I} X_\alpha$ the product of the sets $X_\alpha$. It consists of all functions $x$ that associates each element $\alpha$ of the set $I$ to $x(\alpha) \in X_\alpha$.

Given a point $x \in \prod_{\alpha \in I} X_\alpha$. The function $p_{\alpha}: \prod_{\alpha \in I} X_\alpha \rightarrow X_\alpha$ defined as $p_\alpha(x) = x(\alpha)$ is the $\alpha$th projection.
If for each $\alpha$, $X_\alpha$ is non empty, the function $p_\alpha$ is onto.