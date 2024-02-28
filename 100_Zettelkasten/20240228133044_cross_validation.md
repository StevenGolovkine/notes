---
category: zettelkasten
tags:
  - splines
creation date: 2024/02/28
Write article: false
Done article: false
---
# Leave-one-out Cross-validation (LOOCV)

The idea is to leave out each observation in turn, fit a model to obtain a prediction for it and measure how close that is to the observed observed value.

If $\widehat{y}_{-i}$ is the prediction of $y_i$, based on all others observations, the standard error of predictions is
$$CV = \left(\frac{1}{n}\sum_{i = 1}^n (y_i - \widehat{y}_{-i})^2\right)^{1 / 2}.$$
However, this is computationally expensive as the model has to be estimated $n$ times...
For any linear model with $\widehat{y} = Hy$, it holds that
$$y_i - \widehat{y}_{-i} = \frac{y_i - \widehat{y}_{i}}{1 - h_{ii}}.$$
So, it reduces fitting $n$ models to fitting only one model.
Next, 
1. Choose a grid of values of $\lambda$ (usually not linear).
2. Compute CV for each $\lambda$.
3. Locate the minimum.
