---
category: readingnote
File: "[[yinBayesianNonparametricLearning2022]]"
itemType: note
Status: unread
Date first pass: 24/10/2024
Date second pass: 
Date third pass: 
Clarity: ⭐️⭐️⭐️
Rank: ⭐️⭐️
Figure to add: 
VUE do: false
VUE done: false
Get refs: false
Got refs: false
Find cites: false
Finish cites: false
To be read in details: false
Read in details: false
To be re-implement: false
Re-implemented: false
Write article: false
Done article: false
---
# Title of the paper
Bayesian Nonparametric Learning for Point Processes with Spatial Homogeneity: A Spatial Analysis of NBA Shot Locations

# Learning goal (why read this?)
Learn how to ad non-parametric estimation of the intensity surface of shoots

# Task or problem (what are they solving?)
Estimate non-parametrically the intensity surface

# Data and domain (with what and where?)
20 NBA players in the 2017-2018 season

# Context and relationship (new approach, specialisation of, generalisation of, application of, survey of, example of, ...)
New approach for the analysis shooting charts

# Summary and contributions

The article presents a novel nonparametric Bayesian method for analyzing shot location data in basketball. The approach combines Dirichlet process and Markov random field to learn the underlying intensity surface, which represents the shooting patterns of players.
The proposed method is superior to competing methods due to its ability to encourage local spatial homogeneity while estimating a globally heterogeneous intensity surface. Posterior inferences are performed using an efficient Markov chain Monte Carlo (MCMC) algorithm.
Simulation studies demonstrate the accuracy of the inferences, and application to NBA data from the 2017-2018 regular season reveals interesting insights about shooting patterns among representative players. A comparison with a competing method shows that the proposed approach effectively incorporates spatial contiguity into intensity surface estimation.
This analysis can provide valuable information for coaches, analysts, fans, statisticians, and even players themselves to improve their understanding of shot location data in basketball.

