
---
creation date: 2023-03-28 10:51
last updated: 2023-03-28 10:51
---
# [[20230328105102_expectation_maximisation_algorithm]] - Expectation-Maximisation algorithm
__Tags__: #algorithm-theory  

---
__Contents__: The Expectation-Maximisation algorithm is an iterative algorithm for estimating the parameters that maximise the likelihood of the statistical model.
Consider $X$ the observed data, $Z$ the discrete latent variables and $\theta$ the set of continuous parameters. We note $L(\theta; X, Z) = p(X, Z | \theta)$ the likelihood function. The maximum likelihood estimate is iteratively estimated by these two steps:
	_E-step_: Compute the expected value of the log-likelihood function of $\theta$ with respect to the distribution of $Z$ given $X$ and the current set of parameters $\theta^{(t)}$:
	$$Q(\theta | \theta^{(t)}) = \mathbb{E}_Z(\log p(X, Z | \theta)).$$
	_M-step_: Maximise the quantity
	$$\theta^{(t + 1)} = \arg\max_\theta Q(\theta | \theta^{(t)}).$$
The initialization of the algorithm is done by given some random values to $\theta$. The E-step and M-step are run until convergence criteria has been established.

__References__:
