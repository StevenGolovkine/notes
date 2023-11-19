---
category: readingnote
File: "[[@zhangReviewClusteringMethods2023]]"
itemType: note
Status: read
Date first pass: 31/10/2023
Date second pass: 2023-10-01
Date third pass: 
Clarity: ⭐️⭐️⭐️⭐️
Rank: ⭐️⭐️⭐️⭐️
Figure to add: "2"
VUE do: true
VUE done: true
Get refs: true
Got refs: false
Find cites: true
Finish cites: true
To be read in details: true
Read in details: true
To be re-implement: false
Re-implemented: false
Write article: false
Done article: false
---
# Title of the paper

Review of clustering methods for functional data.

# Learning goal (why read this?)

Understand the current state of clustering functional data.

# Task or problem (what are they solving?)

Identify heterogeneous morphological patterns in functional datasets based on the discrete observations.

# Data and domain (with what and where?)

Data: functional data, could be multivariate and dependent.
Domain: various field of science

# Context and relationship (new approach, specialisation of, generalisation of, application of, survey of, example of, ...)

Survey / overview of clustering functional data in relation to conventional multivariate clustering methods.

# Summary and contributions

Classifies clustering methods into two groups: 
- finite-dimensional clustering (in the vector space): expand the curves into a basis of functions and run the clustering of the coefficients.
	- Model-based clustering: mostly fit a mixture of Gaussian distribution to the coefficients
	- Centroid-based clusteing: based on distance between coefficients
	- Non-parametric Bayesian
- infinite-dimensional clustering (in the function space): based on a dissimilarity measure between the curves (or their derivatives).

![[zhangReviewClusteringMethods2023_fig2.png]]

