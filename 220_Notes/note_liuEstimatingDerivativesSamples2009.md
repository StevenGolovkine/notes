---
category: readingnote
File: "[[@liuEstimatingDerivativesSamples2009]]"
itemType: note
Status: read
Date first pass: 27/11/2023
Date second pass: 
Date third pass: 
Clarity: ⭐️⭐️⭐️⭐️
Rank: ⭐️⭐️⭐️⭐️
Figure to add: 
VUE do: true
VUE done: false
Get refs: false
Got refs: false
Find cites: false
Finish cites: false
To be read in details: false
Read in details: false
To be re-implement: true
Re-implemented: false
Write article: false
Done article: false
---
# Title of the paper

Derivatives for samples of sparsely observed functions, with applucation to online auction dynamics

# Learning goal (why read this?)

Understand how to estimate the derivatives of curves in the context of functional data analysis

# Task or problem (what are they solving?)

They propose an estimation procedure for the derivatives of sparse and noisy curves using the derivatives of the eigenfunctions.

# Data and domain (with what and where?)

Application to online auction dynamics

# Context and relationship (new approach, specialisation of, generalisation of, application of, survey of, example of, ...)

New appoach to estimate the derivatives of curves.

# Summary and contributions

They provide a relationship between the eigenfunctions and its derivatives (eq. 2).
The derivative of the mean is estimated using local polynomials.
We need the partial derivatives of the covariance operator to estimate the derivatives of the eigenfunctions. The partial derivatives are estimated using local polynomials (selection of the bandwitdh using a modified GCV criterion). The scores are estimated using PACE.