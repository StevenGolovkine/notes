
---
creation date: 2023-03-20 14:09
last updated: 2023-03-20 14:09
---
# [[20230320140913_metropolis_hastings]] - Metropolis-Hastings algortihm
__Tags__: #algorithm-theory  #density-estimation

---
__Contents__: The Metropolis-Hastings algorithm is a Markov Chain Monte Carlo method for obtaining a sequence of random samples from a probability distribution.

_Algorithm_: Given $X^{(t)} = x^{(t)}$
	Generate $Y^{(t)} \sim q(y | x^{(t)})$ where $q$ is some distribution that depend (e.g. $\mathcal{N}(x^{(t)}, 1)$).
	Take $X^{(t + 1)} = Y^{(t)}$ with probability $\rho(x^{(t)}, Y^{(t)})$ and $X^{(t + 1)} = x^{(t)}$ with probability $1 - \rho(x^{(t)}, Y^{(t)})$, where 
	$$\rho(x, y) = \min\left(\frac{\widetilde{\pi}(y)}{\pi(x)}\cdot\frac{q(x | y)}{q(y | x)}, 1\right).$$

__References__:

