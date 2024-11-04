---
category: zettelkasten
tags:
  - splines
creation date: 2024/02/29
Write article: false
Done article: false
---
# Array algorithms

In case of large datasets, the usual algorithm to smooth the data may be computationally expensive. For example, if the data have $1000$ rows and $1000$ columns (a common number when working with numbers) and we have a $20$ B-splines basis, the equivalent vector of data will have 1M elements and the Kronecker product of B-splines will have 1M rows and 400 columns, using 3.2Gb of memory.
The normal equations for the least squares solution are
$$\sum_{i}\sum_{j}\sum_{k}\sum_{l} w_{ij}b^{(1)}_{im}b^{(2)}_{jn}b^{(1)}_{ik}b^{(2)}_{jl}\widehat{\alpha}_{kl} = \sum_{i}\sum_{j} w_{ij}b^{(1)}_{im}b^{(2)}_{jn}y_{ij},$$
for all combinations of $m$ and $n$.
The right hand side can be obtained efficiently as $B^{(1)\top}(W \odot Y)B^{(2)}$, but the computation of the left hand side is trickier.

We compute $\mathcal{B}^{(1)} = B^{(1)} \Box B^{(1)}$ amd $\mathcal{B}^{(2)} = B^{(2)} \Box B^{(2)}$. We can show that $\mathcal{B}^{(1)\top}W\mathcal{B}^{(2)}$ contains all the elements of the array $S$ but not in the right position. The idea is to shuffle its elements into the right places of a matrix of the right size.

It is also possible to compute the trace of the hat matrix using this trick.