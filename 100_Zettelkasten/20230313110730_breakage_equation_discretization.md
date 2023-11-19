
---
creation date: 2023-03-13 11:07
last updated: 2023-03-13 11:07
---
# [[20230313110730_breakage_equation_discretization]] - Discretization of the breakage equation

__Tags__: #breakage-equation 

---
__Contents__: Breakage equations can be discretized as the following:
$$\frac{dN_i(t)}{dt} = \sum_{j = i + 1}^n b_{ji}S_jN_j(t) - S_iN_i(t),$$
where $N_i(t)$ is the particle property (here, number of particles) in state $i$ at time $t$. Note that the sum starts at $i + 1$ because the size of the particles can only go in one way (decreasing). 

The idea is to write the breakage equation for a very small time interval $dt = \tau$. The rate of change in the number of distribution of state $i$:
$$\Delta N_i(t) = \sum_{j = i + 1}^n \tau b_{ji}S_jN_j(t) - \tau S_iN_i(t).$$
$N_i(t) + \Delta N_i(t)$ is equal to the number distribution in the future state, and is used to create the transition matrix.

Normalization is needed for the number distribution function but not for the mass distribution. 

__References__:
[[@catakDiscreteSolutionBreakage2010]] - Catak, Bas, Cronin, Fitzpatrick, Byrne - _Discrete Solution of the Breakage Equation Using Markov Chains_ (2010)


