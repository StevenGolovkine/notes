---
category: readingnote
File: "[[@vonluxburgTutorialSpectralClustering2007]]"
itemType: note
Status: read
Date first pass: 30/11/2023
Date second pass: 
Date third pass: 
Clarity: ⭐️⭐️⭐️⭐️⭐️
Rank: ⭐️⭐️⭐️⭐️⭐️
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

A tutorial on spectral clustering

# Learning goal (why read this?)

I want to do spectral clustering for functional data.

# Task or problem (what are they solving?)

They overcome some limitations of classical clustering algorithms.

# Data and domain (with what and where?)

Scalar data points

# Context and relationship (new approach, specialisation of, generalisation of, application of, survey of, example of, ...)

New approach on clustering using a graph

# Summary and contributions

Advantages compared to traditional approaches: better results, simple to implement and solved by standard linear algebra methods.

The idea is to represent the data as graph, where each vertex is a data point and each edge is the similarity between the two data points. The degree of a vertex is the sum of all the edge that starts from it.

Construction of the graph:
- $\epsilon$-neighborhood graph: connect points with distances smaller than $\epsilon$.
- $k$-nearest neighbor graphs: connect points with the $k$ smallest distances.
- fully connected graph: connect points with positive similarity (the neighborhood has to be controlled by a parameters, e.g. kernel function)

Graph Laplacian:
- Defined as the difference between the degree matrix (diagonal) and the matrix of similarities.
- Their eigencomponents have interesting properties. In particular, the multiplicity of the eigenvalue 0 is equals to the number of connected components in the graph.

Algorithm:
1. Construct similarity graph
2. Compute Laplacian matrix
3. Diagonalise the Laplacian matrix and get the eigenvectors.
4. Create a matrix of eigenvectors.
5. Cluster the rows of the previous matrix using $k$-means.