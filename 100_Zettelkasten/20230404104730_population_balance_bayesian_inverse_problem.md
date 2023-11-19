
---
creation date: 2023-04-04 10:47
last updated: 2023-04-04 10:47
---
# [[20230404104730_population_balance_bayesian_inverse_problem]] - Estimation of parameters in population balance models using Bayesian inverse problem approach
__Tags__: #population-balance #bayesian-analysis  

---
__Contents__: The Bayesian approach is used to estimate the distribution of the parameters and not just the parameter values. It needs experimental data. One advantage is to incorporate priors knowledge to improve the reliability of the model prediction and quantify uncertainties (useful for decision making and risk assessment).

Bayesian inversion provides a powerful framework for estimating model parameters and their uncertainties in a statistically rigourous way.
The steps for the Bayesian approach are
1. Specifying a prior distribution that represents our knowledge on the data. In practice, we just have to make sure that the parameters are positive.
2. Update this distribution (Bayes theorem) to obtain a posterior distribution using information from the experimental data (likelihood).
3. Use MCMC to sample from the posterior distribution. Sampling can be performed using Metropolis-Hastings ([[20230320140913_metropolis_hastings]]) or Wang-Landau algortihms.

We have to deal with problems the data (sampling error, images resolution, innacurate size determination). Error propagation is used to determine the uncertainty in model parameters estimates obtained using MCMC algorithm; the uncertainty is then propagated through the model to determine its effect on model predictions.

_How to compute the likelihood?_ Solve the forward model with a given set of parameters and compare its prediction with the data (asuming that the measurement error are normally distributed with mean $0$ and know variance).

_Example_:
* Prototype IR(0) on nanoparticle formation system (growth) ([[@longEstimatingReactionParameters2022]]).
* Jet milling process ([[@kastnerBayesianParameterEstimation2013]]).

**Questions**:
* Could we do a mix between MC and Bayesian methods? Especially, use MC to do the forward pass and Bayesian for the backward pass.
* Could we use Bayes factors to compare the different models?

__References__:
[[@longEstimatingReactionParameters2022]] - Long, Bangerth, Handwerk, Whitehead, Shipman, Finke - _Estimating reaction parameters in mechanism-enabled population balance models of nanoparticle size distributions: A Bayesian inverse problem approach_ (2022)
[[@kastnerBayesianParameterEstimation2013]] - Kastner, Braumann, Man, Mosbach, Brownbridge, Akroyd, Kraft, Himawan - _Bayesian parameter estimation for a jet-milling model using Metropolis–Hastings and Wang–Landau sampling_ (2013)