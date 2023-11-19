
---
creation date: 2023-04-04 10:49
last updated: 2023-04-04 10:49
---
# [[20230404104909_population_balance_abc]] - Estimation of parameters in population balance models using Approximate Bayesian Computation (ABC)
__Tags__: #population-balance #bayesian-analysis  

---
__Contents__: ABC can be used to simultaneously select models and estimate parameters in population balance models.

Model selection is important. Different models have different assumptions and parameters. Selecting a model will improve the prediction of particle size.
The idea is to use a likelihood-free inference approach which compare simulated data from the model with the experimental data and accept or reject the parameter values. This allows simultaneous model selection and parameters estimation.

_Steps_
1. Define the model (based on physical principles)
2. Define prior distribution
3. Simulate data and compare with experimental data
4. Accept or reject parameters values
5. Approximate posterior distribution
6. Perform inference

**Questions:**
* Can we use ABC and MC simulataneously?

__References__:
[[@mouraEstimationParametersSelection2022]] - Moura, Viegas, Tavares, Macedo, Estumano - _Estimation Of Parameters And Selection Of Models Applied To Population Balance Dynamics Via Approximate Bayesian Computational_ (2022)


