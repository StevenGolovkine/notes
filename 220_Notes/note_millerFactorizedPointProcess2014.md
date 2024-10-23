---
category: readingnote
File: "[[millerFactorizedPointProcess2014]]"
itemType: note
Status: read
Date first pass: 23/10/2024
Date second pass: 
Date third pass: 
Clarity: 
Rank: 
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
Factorized point process intensities: A spatial analysis of professional basketball

# Learning goal (why read this?)
Learn about the application of point process in basketball.

# Task or problem (what are they solving?)
Analyze the underlying spatial structure that governs shot selection among basketball players in the NBA.

# Data and domain (with what and where?)
Made and missed field goal attempt locations from half of the games in the 2012-2013 NBA regular season.

# Context and relationship (new approach, specialisation of, generalisation of, application of, survey of, example of, ...)
Application of point process modeling and non-negative matrix factorization to shooting patterns.

# Summary and contributions

The paper describes a machine learning approach to analyze shot selection among professional basketball players in the NBA. The authors model shot attempt data as a point process and use non-negative matrix factorization (NMF) to create a low-dimensional representation of offensive player types. This spatial decomposition summarizes the shooting habits of NBA players, resulting in intuitive descriptions of player types that can be used to model other spatial effects, such as shooting accuracy.

* Background on: Gaussian process, Poisson process, Log-gaussian Cox process and Non-negative matrix factorization
* Approach:
	* Discretized the court
	* Fit intensity (= density) surface using LGCP
	* Normalized intensity surface for each player
	* Perform NMF
* Defined efficiency a shooting frequency considering spatial location