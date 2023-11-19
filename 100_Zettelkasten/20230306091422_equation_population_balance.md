
---
creation date: 2023-03-06 09:14
last updated: 2023-03-13 10:09
---
# [[20230306091422_equation_population_balance]] - General equation for population balance models

__Tags__: #population-balance 

---
__Contents__: A general equation governs population balance models. The equation is given by

$$\frac{\partial n(t, u)}{\partial t} = -\frac{\partial G(t, u)n(t, u)}{\partial u} + B_{nuc}(t, u) + Q_{agg}^{\pm}(t, u) + Q_{brk}^{\pm}.$$
where:
* $n(t, u)$ refers to the distibution of the number of particles of mass $u$ at time $t$.

The first part of the equation is viewed as the rate of surface growth, the second term is the nucleation term, the third term is the aggregation term and the last term is the breakage term.
We define the moments of the distribution as
$$\mu_i(t) = \int_0^{\infty} u^i n(t, u).$$
This corresponds to the expectation of random variables. Physical explanations are given for the first moments. For $i = 0$, it corresponds to the number of particles and for $i = 1$, we get the mass.
For some particular cases, analytical solutions are derived. Most of them use analytical methods ([[20230306095019_numerical_methods_population_balance]]). Machine learning techniques can also be employed ([[20230404151225_machine_learning_population_balance]]).


A set of parameters usually governs population balance equations. The estimation of these parameters could be done using:
* Bayesian inverse problem approach ([[20230404104730_population_balance_bayesian_inverse_problem]])
* Approximate Bayesian Computation ([[20230404104909_population_balance_abc]])

__References__:



