---
category: zettelkasten
tags:
  - splines
creation date: 2024/02/27
Write article: false
Done article: false
---
# Effective dimension

We have $\widehat{y} = Hy$ where $H = B(B^\top W B + \lambda D^\top D)^{-1}B^\top W$. The effective dimension of the model is equal to $\text{tr}(H)$.

Using cyclic permutation, a computationally more attractive way to compute the effective dimension is
$$\text{tr}(H) = \text{tr}(B^\top WB(B^\top W B + \lambda D^\top D)^{-1}).$$




