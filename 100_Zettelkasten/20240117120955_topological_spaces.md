---
category: zettelkasten
tags:
  - "#topology"
creation date: 2024/01/17
Write article: false
Done article: false
---
# Topological spaces

Topological spaces are created by discarding the notion of distance from metric spaces and characterize the different notions using open sets.

Let $X$ be a set and $\mathfrak{S}$ a collection of subsets of $X$. The pair of objects $(X, \mathfrak{S})$ is a topological space, provided that:
1. $X \in \mathfrak{S}$
2. $\emptyset \in \mathfrak{S}$
3. If $O_1, \dots, O_n \in \mathfrak{S}$, then $O_1 \cap \cdots \cap O_n \in \mathfrak{S}$.
4. If for each $\alpha \in I$, $O_\alpha \in \mathfrak{S}$, then $\bigcup_{\alpha \in I} O_\alpha \in \mathfrak{S}$.
The set $X$ is the unerlying set. The collection $\mathfrak{S}$ is the topology on the set $X$. The elements of $\mathfrak{S}$ are called open sets.

If $\mathfrak{S}$ is the collection of open sets of a metric space $(X, d)$, then $(X, \mathfrak{S})$ is the topological space associated with the metric space $(X, d)$. Thus, every metric space is a topological space, but the contrary is not true.

**For example**:
* Let $X$ be a set and $\mathfrak{S} = \{X, \emptyset\}$. Then $(X, \mathfrak{S})$ is a topological space.
* Let $X$ be a set and $\mathfrak{S} = 2^X$ be the collection of all subsets of $X$. Then $(X, \mathfrak{S})$ is a topological space, called the discrete topology.

**Be careful: the notion of open ball does not exists in a topological space.**

A function $f$ from a topological space $(X, \mathfrak{S})$ to a topological space $(Y, \mathfrak{S}^\prime)$ is a function $f: X \rightarrow Y$.