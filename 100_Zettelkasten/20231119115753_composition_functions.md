---
category: zettelkasten
tags:
  - "#topology"
  - "#sets"
creation date: 2023/11/19
Write article: false
Done article: false
---
# Composition of functions

Given two functions, $f: A \rightarrow B$ and $g: B \rightarrow C$, the composition of $f$ and $g$ is the function $h: A \rightarrow C$ such that $\forall x \in A, h(x) = g \circ f (x)$.

![[composition_figure_1.png|200]]

The composition of functions written for a finite number of functions, as long as their domain and range are well defined. For example, let $f: A \rightarrow A$, the composition of the function $n$ times is
$$f^{(n)}(x) = \underbrace{f \circ f \circ \cdots \circ f}_{n \text{ times}} (x).$$
Composition can be represented as diagrams. Arrows represent a function from set to another.

![[composition_figure_2.png|200]]

If the composition of functions are equal from one set to another, we say that the diagram is commutative. For example, in the Figure above, the diagram is commutative if $h$ and $g \circ f$ are equal.