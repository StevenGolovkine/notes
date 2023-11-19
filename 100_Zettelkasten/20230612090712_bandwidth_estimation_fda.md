
---
creation date: 2023-06-12 09:07
last updated: 2023-06-12 09:07
---
# [[20230612090712_bandwidth_estimation_fda]] - Bandwidth estimation in functional data
__Tags__: #functional-data #adaptive-optimal-smoothing 

---
__Contents__: The optimal bandwidth for the $p$ order local polynomial kernel reconstruction of the curve $\widehat{f}(t)$ is
$$h = \mathcal{O}(n^{-\delta / (2p + 3)}).$$
The bandwidth selection can be done using generalized cross validation (GCV) as the mean over all the curves. For one curve,
$$\text{GCV}_i(h) = y_i^\top\left(I - A_i\right)^\top\left(I - A_i\right)y_i \times \left(1 - \frac{\text{tr}(A_i)}{M_i}\right)^{-2},$$
which can be minimized over a grid of $h$.

The GCV is then 
$$\text{GCV}(h) = \frac{1}{N}\sum_{n = 1}^N \text{GCV}_i(h).$$
__References__:
[[@zhangStatisticalInferencesFunctional2007a]] - J.-T. Zhang, J. Chen - *Statistical inferences for functional data* (2007)