---
category: readingnote
File: "[[grithFunctionalPrincipalComponent2018]]"
itemType: note
Status: read
Date first pass: 20/11/2023
Date second pass: 
Date third pass: 
Clarity: ⭐️⭐️⭐️⭐️
Rank: ⭐️⭐️⭐️⭐️
Figure to add: 
VUE do: true
VUE done: false
Get refs: true
Got refs: false
Find cites: true
Finish cites: false
To be read in details: false
Read in details: false
To be re-implement: false
Re-implemented: false
Write article: false
Done article: false
---
# Title of the paper

Functional principal component analysis for derivatives of multivariate curves

# Learning goal (why read this?)

Understand how to estimate the derivatives of curves (eventually multidimensional)

# Task or problem (what are they solving?)

Propose methods to estimate derivatives

# Data and domain (with what and where?)

Functional data (eventually multidimensional).
Applied to the DAX 30 stock index.

# Context and relationship (new approach, specialisation of, generalisation of, application of, survey of, example of, ...)

New approaches to estimate the derivatives of curves.

# Summary and contributions

Two methods:
- Estimate the derivatives, and then compute the eigenelements.
- Estimate the eigenelements of the curves and then compute the derivatives of the eigenfunctions.

They use the Gram matrix to estimate the eigencomponents. They use local polynomial regression to handle noisy and discrete observations in the estimation of the Gram matrix.

They propose asymptotic theory and it can be used to do asymptotic theory in our Gram paper [[@golovkineUseGramMatrix2023]]. They add the assumption of the factor model (that the curves can be expanded into a finite basis of functions).

They applied the methodology to two-dimensional call option.
