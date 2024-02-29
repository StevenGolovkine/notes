---
category: zettelkasten
tags:
  - splines
creation date: 2024/02/28
Write article: false
Done article: false
---
# Tensor Product Models

Tensor product models are generalizations of the B-splines basis and penalties that allows interactions in two dimensions.
There will be two penalties, one down all columns and another along all rows. The penalties can have different values of $\lambda$ in the different dimensions, allowing anisotropic smoothing.

Let $Y \in \mathbb{R}^{n \times m}$ be the data matrix and $W \in \mathbb{R}^{n \times m}$ be the weights associated to the data. Let $(i, j)$ be the coordinate of a point in $Y$.
Based on the row $i$, we can compute the B-splines basis $B^{(1)} \in \mathbb{R}^{n \times b_1}$ and based on the column $j$, we can compute the B-splines basis $B^{(2)} \in \mathbb{R}^{m \times b_2}$. The tensor product between the elements of the basis are $b^{(1)}_{ik_1}b^{(2)}_{jk_2}$, where $i = 1, \dots, n, j = 1, \dots, m, k_1 = 1, \dots, b_1$ and $k_2 = 1, \dots, b_2$. The expected value of $y_{ij}$ is given by
$$\mathbb{E}(y_{ij}) = \sum_{k_1 = 1}^{b_1}\sum_{k_2 = 1}^{b_2} b^{(1)}_{ik_1}b^{(2)}_{jk_2} \alpha_{k_1k_2},$$
and the coefficients form a matrix $A = [\alpha_{k_1k_2}] \in \mathbb{R}^{b_1 \times b_2}$. We can rewrite this equation in a matrix form
$$\mathbb{E}(Y) = B_1AB_2^\top.$$
This hold in higher dimension, but the notation gets trickier to write.

For a matrix $U$, we note $\lvert\!\lvert U \rvert\!\rvert_F^2$ the squared Frobenius norm (sum of the squares of all the elements of the matrix).
For two matrix $U$ and $V$, we note $U \odot V$ the element-wise product of $U$ and $V$.

**Estimation of the matrix coefficients** $A$:
We define the objective function
$$S = \lvert\!\lvert W^{1 / 2} \odot (Y - \mathbb{E}(Y)) \rvert\!\rvert_F^2 = \lvert\!\lvert W^{1 / 2} \odot (Y - B_1AB_2^\top) \rvert\!\rvert_F^2.$$
The matrix $W^{1 / 2}$ is the element-wise square-root matrix. The trick to minimize this function is to vectorize the matrices and using the Kronecker product of the B-splines basis.
Let $\alpha = \text{vec}(A) \in \mathbb{R}^{b_1b_2 \times 1}, w = \text{vec}(W) \in \mathbb{R}^{nm \times 1}, y = \text{vec}(Y) \in \mathbb{R}^{nm \times 1}$  and $B = B_1 \otimes B_2 \in \mathbb{R}^{nm \times b_1b_2}$. Wer can then rewrite the objective function as
$$S = \left(y - B\alpha\right)^\top \text{diag}(w) \left(y - B\alpha\right).$$
The solution is then the usual least-square solution 
$$\widehat{\alpha} = \left(B^\top\text{diag}(w) B\right)^{-1}B^\top \text{diag}(w)y.$$
Finally, we can reshape the vector $\widehat{\alpha}$ into a matrix $\widehat{A}$.

**What happen if the data are not on a grid?**
We observe $N$ quadruples $(i, j, y, w)$ where $i$ and $j$ are arbitrary coordinate positions. Similarly to the grid case, we compute the B-splines basis $B^{(1)}$ and $B^{(2)}$. The expected value of $y_{i}, i = 1, \dots, N$ is given by
$$\mathbb{E}(y_{i}) = \sum_{k_1 = 1}^{b_1}\sum_{k_2 = 1}^{b_2} b^{(1)}_{ik_1}b^{(2)}_{ik_2} \alpha_{k_1k_2},$$
The objective function $S$ remains the same but the definition of $B$ change. The rows of $B$ are now the Kronercker product of the corresponding rows of $B^{(1)}$ and $B^{(2)}$:
$$B = B^{(1)} \Box B^{(2)} = \left(B^{(2)} \otimes 1_{b_1}^\top\right) \odot \left(1_{b_2}^\top \otimes B^{(1)}\right).$$
