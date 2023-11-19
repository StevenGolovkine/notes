---
category: readingnote
File: "[[@galeanoMahalanobisDistanceFunctional2015]]"
itemType: note
Status: read
Date first pass: 31/10/2023
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
To be read in details: true
Read in details: false
To be re-implement: true
Re-implemented: false
Write article: true
Done article: false
---
# Title of the paper

The Mahalanobis distance for functional data with applications to classification

# Learning goal (why read this?)

Understand how Mahalanobis distance for functional data may be defined

# Task or problem (what are they solving?)

Introduced the Mahalanobis (semi) distance for functional data + classification

# Data and domain (with what and where?)

Data: Univariate functional data

# Context and relationship (new approach, specialisation of, generalisation of, application of, survey of, example of, ...)

Generalisation of Mahalanobis distance to functional data

# Summary and contributions

Properties of the distance:
* consider the correlation structure of the data
* scale-invariant
Note that the Mahalanobis distance can be written in terms of the PC scores.
Define the inverse of the covariance operator, that exists only in some conditions (proposition 1 is important).
Functional Mahalanobis distance between curves = Euclidean norm of he standardised PC scores.

Classification models:
* $k$-NN
* Centroid procedure
* Functional linear and quadratic bayes classification rules