---
category: readingnote
File: "[[ievaCovariancebasedClusteringMultivariate2016]]"
itemType: note
Status: unread
Date first pass: 07/11/2023
Date second pass: 
Date third pass: 
Clarity: ⭐️⭐️
Rank: ⭐️
Figure to add: algorithm 1
VUE do: true
VUE done: true
Get refs: true
Got refs: true
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

Covariance-based clustering in multivariate and functional data analysis

# Learning goal (why read this?)

Understand clustering using covariance operator

# Task or problem (what are they solving?)

Propose a clustering algorithm for population that differ in their covariance

# Data and domain (with what and where?)

Data: Multivariate and functional data
Application: biostatistics / genomics

# Context and relationship (new approach, specialisation of, generalisation of, application of, survey of, example of, ...)

Two-samples problem adapted to clustering

# Summary and contributions

* Distance between covariance operators.
* This distance is used to search the partition that maximise the class-specific covariances.
* Provide an efficient algorithm to perform the search using shrinkage estimator of the covariance (max-swap algorithm, [[@ledoitWellconditionedEstimatorLargedimensional2004]])

![[ievaCovariancebasedClusteringMultivariate2016_algo1.png]]