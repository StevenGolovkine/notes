
---
creation date: 2023-06-12 08:45
last updated: 2023-06-12 08:45
---
# [[20230612084505_noise_functional_data]] - Estimation of the noise function
__Tags__: #functional-data #noise-reduction 

---
__Contents__: The estimation of the noise variance function $\sigma^2(t)$ is based on the residuals and can be estimated using local polynomials smoothing.
Let the residuals be
$$\widehat{\varepsilon}_{ij} = y_{ij} - \widehat{f}_i(t_{ij}).$$
$$\widehat{\sigma^2}(t) = \left(\sum_{i = 1}^N\sum_{j = 1}^{M_i} K_\lambda(t, t_{ij})\right)^{-1}\left(\sum_{i = 1}^N\sum_{j = 1}^{M_i} K_\lambda(t, t_{ij})\widehat{\varepsilon}^2_{ij}\right)$$

__References__:


