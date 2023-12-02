---
category: zettelkasten
tags:
  - "#topology"
  - function
  - sets
creation date: 2023/12/01
Write article: false
Done article: false
---
# Construction of the sinus function

Consider the set $A = (0, \pi / 2)$. For each $\theta \in A$, we note $\Delta_\theta$ the right triangle with one of the acute angles is $\theta$ radians. Let $f: A \rightarrow \mathbb{R}$ be the function such that it is defined as the ratio between the side of the triangle opposite to $\theta$ and the hypotenuse. This function is the sinus function restricted to $A$.

![[sinus_figure_1.png|200]]

We can extend this defintion to each $\theta \in \mathbb{R}$. Let $\mathcal{C} = \{(a, b) / \sqrt{a^2 + b^2} = 1\}$ be the set of points in $\mathbb{R}^2$ whose distance from the origine is $1$ (know as the unit circle).  For each $\theta \in \mathbb{R}$, let $(a, b)_{\theta}$ be the point in $\mathcal{C}$ such that it represents an angle of magnitude $\theta$ radians. Defining the function $f$ as before (the hypotenuse is equal to $1$), we extend the sinus function to $\mathbb{R}$.

![[sinus_figure_2.png|200]]

The sinus function may also be seen as the projection of the point $(a, b)_\theta$ onto the second component, resulting in
$$f(\theta) = b.$$
Similarly, the cosinus function is the projection of the point $(a, b)_{\theta}$ onto the first component, resulting in
$$f(\theta) = a.$$
