---
category: zettelkasten
tags:
  - "#dynamics"
creation date: 2024/11/04
Write article: false
Done article: false
---
# Dynamical systems

Dynamical systems refer to observations distributed over a continuum. We differentiate between deterministic (the system depend on non-random quantities) and stochastic (the system depend on random quantities) systems. Usually, we consider $x$ a function of position (named states, paths or trajectories). 

Systems incorporate parameters $\theta$ that have to be estimated from the data (and get confidence intervals). 
Dynamical systems are defined by equations involving one or more derivatives.

Differential equation of order $m$ can be expressed as:
$$D^m x = f(x, Dx, \dots, D^{m - 1}x)$$
The $m$ is the order of the equation. In the case of several variables together, the letter $d$ will refer to the dimension of the system.
We note $L$ the differential operator associated with the dynamic system.

Type of differential equations:
* Linear ([[20241104141832_linear_differential_equation]])
* Nonlinear ([[20241104141945_nonlinear_dynamical_systems]])
* Partial ([[20241104142037_partial_differential_equations]])