
---
creation date: 2023-06-06 10:58
last updated: 2023-06-06 10:58
---
# [[20230606105824_robust_kernel_smoothing]] - Robust kernel smoothing methods
__Tags__: #non-parametric-statistics  

---
__Contents__: An idea to robustify local polynomial smoothers ([[20230606101448_kernel_smoothing_methods]]) is to update the weights using the residuals.

Procedure:
1. Perform usual LP
2. Compute robustness weights $\delta_k = B(e_k / 6s)$ where $B$ is the bi-sqaure kernel, $e_k$ are the residuals and $s$ is the median of the absolute values of the residuals.
3. Compute estimation with weights $\delta_k K_\lambda(x_0, x_i)$
4. Do it multiple times

How to choose:
* Polynomial order: degree $1$ to balance between computational ease and flexibility
* Kernel: tricube kernel
* Number of iteration for robustness: experimentation say $2$
* Bandwidth: PRESS procedure adapted to local polynomial

__References__:
[[@clevelandRobustLocallyWeighted1979a]] - Cleveland - _Robust Locally Weighted Regression and Smoothing Scatterplots_ (1979

