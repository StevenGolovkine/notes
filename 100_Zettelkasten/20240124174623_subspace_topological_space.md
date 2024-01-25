---
category: zettelkasten
tags:
  - topological-space
creation date: 2024/01/24
Write article: false
Done article: false
---
# Subspaces of topological spaces

Let $(X, \mathfrak{S})$ be a topological space. Given a subset $Y$ of $X$, we can create a topological space using open sets of $X$.

Definition: $(Y, \mathfrak{S}^\prime)$ is a subspace of $(X, \mathfrak{S})$ if $Y \subset X$ and if the open subsets of $Y$ are precisely the subsets $O^\prime$ of the form $O^\prime = O \cap Y$ for some open subset $O$ of $X$. ($O^\prime$ is relatively open in $Y$.)

Define the collection $\mathfrak{S}^\prime$ of subset of $Y$ as the collection of subsets $O^\prime$ of $Y$ of the form $O^\prime = O \cap Y$, where $O \in \mathfrak{S}$. Then $(Y, \mathfrak{S}^\prime)$ is a topological space and therefore a subspace of $(X, \mathfrak{S})$ provided $Y \neq \emptyset$. ($\mathfrak{S}^\prime$ is induced by $\mathfrak{S}$ and is the relative topology on $Y$.)

Let $x \in Y$. A subset $N^\prime$ of $Y$ is a relative neighborhood of $x$ if and only if $N^\prime = N \cap Y$, where $N$ is a neighborhood of $x$ in $X$.

A subset $F^\prime$ of $Y$ is relatively closed in $Y$ if and only if $F^\prime = F \cap Y$, for some closed subset $F$ of $X$.

If $(Y, \mathfrak{S}^\prime)$ is subspace of $(X, \mathfrak{S})$, then the inclusion mapping $i: Y \rightarrow X$ is continuous.