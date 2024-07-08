---
category: readingnote
File: "[[banfieldModelBasedGaussianNonGaussian1993]]"
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
To be re-implement: false
Re-implemented: false
Write article: false
Done article: false
---
# Title of the paper

Model-based Gaussian and Non-Gaussian Clustering

# Learning goal (why read this?)

Understand how non-gaussian data are handled in clustering.

# Task or problem (what are they solving?)

Cluster non-gaussian data

# Data and domain (with what and where?)

Non-gaussian data

# Context and relationship (new approach, specialisation of, generalisation of, application of, survey of, example of, ...)

Generalisation of the clustering algorithms

# Summary and contributions

They assume a mixture model for the data. They propose three generalisations:
- Gaussian mixture with different covariances. The idea is parametrise the different covariances using the eigenvalues decomposition.
- Non-Gaussian clustering with Poisson noise. The idea is to use local parametrisation and compute the likelihood for a given distributions.
- Bayesian approach to choose the number of clusters. The idea is to choose between competing models.