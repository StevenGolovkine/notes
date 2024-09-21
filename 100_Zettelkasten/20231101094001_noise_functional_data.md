---
category: zettelkasten
tags:
  - functional-data
  - noise-reduction
creation date: 2023/11/01
Write article: false
Done article: false
---
# How is the noise specified in functional data models?

## Noise added as a realisation of a stochastic process

For each $1 \leq i \leq N$, we denote by $X_i$ a realisation of the stochastic process $X$ and $\varepsilon_i$ a realisation of the stochastic process $\varepsilon$. The model is given by
$$
Y_i(t) = X_i(t) + \varepsilon_i(t), \quad t \in \mathbb{R},
$$
The process $\varepsilon$ could be a Gaussian process or a Browmian motion for example. **But**, it can not be a process such that 
$$\mathbb{E}[\epsilon_i(t)] = 0, \quad\text{and}\quad \mathbb{E}[\epsilon_i^2(t)] = \sigma_i^2,$$
as there is no measurable process equivalent to $\epsilon_i$ [[see Example 1.2.5, @kallianpurStochasticFilteringTheory1980]], or such that
$$\mathbb{E}[\epsilon_i(t)] = 0, \quad\text{and}\quad \mathbb{E}[\epsilon_i^2(t)] = \sigma_i^2(t),$$
(I'm actually not sure about that claim)

## Noise added on the measurements at fixed time of the realisations of the process

For each $1 \leq i \leq N$, and given a positive integer $M_i$, let $T_{im} \in \mathbb{R}, 1 \leq m \leq M_i$, be the observation times for the curve $X_i$. The observations associated with a curve $X_i$ consist of the pairs $(Y_{im}, T_{im}) \in \mathbb{R} \times \mathbb{R}$ where
$$Y_{im} = X_i(T_{im}) + \varepsilon_{im}, \quad 1 \leq m \leq M_i, 1 \leq i \leq N,$$
where $\varepsilon_{im}$ is an independent (centered) error variable. The notation $X_{it}$ is used for the value at a generic point $t \in \mathbb{R}$ of the realisation $X_i$ of the process $X$, while $X_i(T_{im})$ denotes the measurement at $T_{im}$ of this realisation.


From [[@kallianpurStochasticFilteringTheory1980]], *In statistical problems of prediction and filtering it is important to have a useful mathematical model of a "white noise" process. In the case of problems involving discrete time (that is, when $T$ is at most countably infinite), white noise (or Gaussian white noise) can simply be taken to be a sequence of independent, identically distributed (Gaussian) random variables. In view of Example 1.2.5, one has to look elsewhere for an appropriate model of a white noise process. The Wiener process turns out to be a convenient and versatile model when the noise is Gaussian. Other models of white noise [...] have been considered in the literature (such as generalized processes or finitely additive white noise measures) [...].*


