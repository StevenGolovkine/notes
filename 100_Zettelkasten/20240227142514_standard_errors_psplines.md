---
category: zettelkasten
tags:
  - splines
creation date: 2024/02/27
Write article: false
Done article: false
---
# Standard errors

The (Bayesian) covariance matrix of the estimated coefficients is
$$\widehat{C} = \text{Cov}(\widehat{\alpha}) = \widehat{\sigma}^2 (B^\top W B + \lambda D^\top D)^{-1},$$
where $\widehat{\sigma}^2 = \lvert\!\lvert y - \widehat{y} \rvert\!\rvert^2 / (n - \text{tr}{H})$. 
The diagonal of $B\widehat{C}B^\top$ gives the variane of the fitted values $\widehat{y}$. Taking the square-root of these values, we build error bands.

