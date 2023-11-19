
---
creation date: 2023-03-13 11:01
last updated: 2023-03-13 11:01
---
# [[20230313110112_markov_chain_for_breakage]] - Markov chains for breakage equations

__Tags__: #breakage-equation #markov-chains 

---
__Contents__: Markov chains can be used to model breakage equation. It is based on a discretization of the equation ([[20230313110730_breakage_equation_discretization]]). The aim is to estimate the particle size distribution at each time step.

The different elements of the Markov chain are given by:
* State space: discrete values (center of the bins) of particle property (number, mass, ...).
* State probability vector: values of particles property over the state space.
* Transition matrix: transition probabilities to go from one state to another.

More states give better results. The constant parameters are estimated by machine learning approaches to minimized the squared error between the model and the measurements.

**Application of Markov chain for breakage equation**:
* Aggregated food products passing through a pneumatic conveying pipeline rig ([[20230313112753_example_breakage_food_products]]).
* Particulate mixing problems ([[20230313114851_example_breakage_mixing]]).

**Questions**:
* Could it be extended to time-dependent or state-dependent Markov chain?
* Could it be possible to add uncertainties around the distributions?

__References__:
[[@catakDiscreteSolutionBreakage2010]] - Catak, Bas, Cronin, Fitzpatrick, Byrne - _Discrete Solution of the Breakage Equation Using Markov Chains_ (2010)


