---
category: readingnote
File: "[[yaoFunctionalDataAnalysis2005]]"
itemType: note
Status: read
Date first pass: 27/11/2023
Date second pass: 
Date third pass: 
Clarity: ⭐️⭐️⭐️⭐️
Rank: ⭐️⭐️⭐️⭐️⭐️
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

Functional data analysis for sparse longitudinal data

# Learning goal (why read this?)

Understand how to estimate the eigencomponents for sparse functional data

# Task or problem (what are they solving?)

Propose an estimation method for the eigencomponents for sparse functional data

# Data and domain (with what and where?)

Sparse functional data
Application to CD4 and Yeast Cell Cycle Gene expression profile.

# Context and relationship (new approach, specialisation of, generalisation of, application of, survey of, example of, ...)

New approach for the eigencomponents for sparse functional data

# Summary and contributions

For sparse functional data, they estimate the eigencomponents (eigenvalues, eigenfunctions and scores) of the observations.
- Estimate the mean and covariance functions using local polynomials.
- Estimate the noise using the difference between the raw and smoothed diagonal of the covariance.
- Under Gaussian assumption, they derive the scores (and provide confidence bands).
- Derive confidence bands for individual trajectories (based on the confidence bands for the scores).
