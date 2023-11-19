
---
creation date: 2023-06-06 10:14
last updated: 2023-06-06 10:14
---
# [[20230606101448_kernel_smoothing_methods]] - Kernel smoothing methods
__Tags__: #non-parametric-statistics  

---
__Contents__: The terms *Local polynomial kernel smoothing* and *locally weighted regression regression* refer to the same method.

Considering a regression settings $y = f(x) + \varepsilon$. We aim to estimate the function $f: \mathbb{R}^p \rightarrow \mathbb{R}$. The idea is to fit a simple (but different) model to each point in $\mathbb{R}^p$. Let $x_0$ be the point where we want to estimate $f$. The estimation of $\widehat{f}(x_0)$ is performed using the points that are "close" to $x_0$ and result in a smooth function. The neighborhood of $x_0$ is chosen using a weighting function $K_\lambda(x_0, x_i)$, _the kernel_, that depends on a parameter $\lambda$, _the bandwidth_.

* kNN has this idea of localization, but it results to discontinuity.
* Nadaray-Watson estimator is continuous but contant.
$$\widehat{f}(x_0) = \left(\sum_{i = 1}^N K_\lambda(x_0, x_i)\right)^{-1}\sum_{i = 1}^N K_\lambda(x_0, x_i)y_i, \quad\text{where}\quad K_\lambda(x_0, x_i) = D\left(\frac{|x_0 - x_i|}{\lambda}\right)$$
The function $D$ is a function with some properties.
* Local linear estimators are continuous and not constant. It solves the weighted least-squares problem at **each target point** $x_0$:
$$\min_{\alpha, \beta} \sum_{i = 1}^N K_\lambda(x_0, x_i)\left(y_i - \alpha(x_0) - \beta(x_0)x_i\right)^2.$$
We use this model to evaluate the fit at a single point $x_0$. We can write down a closed-form solution for this minimization problem:
$$\widehat{f}(x_0) = b(x_0)^\top \left(B^\top W(x_0) B\right)^{-1} B^\top W(x_0)y,$$
where $B$ is a design matrix and $W(x_0)$ is a diagonal matrix with kernel values as entries. 

This can be extended to local polynomial regression. In that case, the minimization problem is written
$$\min_{\alpha, \beta_j, j = 1, \dots, d} \sum_{i = 1}^N K_\lambda(x_0, x_i)\left(y_i - \alpha(x_0) - \sum_{j = 1}^d \beta_j(x_0)x_i^j\right)^2.$$
This can be easily extend to $\mathbb{R}^p$ using 
$$K_\lambda(x_0, x_i) = D\left(\frac{||x_0 - x_i||}{\lambda}\right),$$
where $|| \cdot ||$ is the Euclidean norm.

There is a bias/variance tradeoff concerning the choice of the bandwidth $\lambda$. Large $\lambda$ results in small variance and large bias, and small $\lambda$ results in small bias and large variance.

Note that local polynomial regression performs boundary correction to the desired order in any dimension.

__References__:
[[@hastieElementsStatisticalLearning2009]] - Hastie, Tibshirani and Friedman - _The Elements of Statistical Learning: Data Mining, Inference, and Prediction, Second Edition_ (2009)


