---
category: readingnote
File: "[[zuccolottoSpatialPerformanceAnalysis2023]]"
itemType: note
Status: unread
Date first pass: 29/10/2024
Date second pass: 
Date third pass: 
Clarity: ⭐️⭐️⭐️⭐️
Rank: ⭐️⭐️⭐️
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
Spatial performance analysis in basketball with CART, random forest and extremely randomized trees

# Learning goal (why read this?)
Work on the shooting chart but not to categorize players.

# Task or problem (what are they solving?)
Estimate the scoring probability using CART

# Data and domain (with what and where?)
2020-2021 NBA season

# Context and relationship (new approach, specialisation of, generalisation of, application of, survey of, example of, ...)
New approach to estimate scoring probabilties

# Summary and contributions

The query proposes tools for spatial performance analysis in basketball, aiming to represent maps of the court visualizing areas with different levels of scoring probability for a player or team.
To achieve this, the query suggests using algorithmic modeling techniques. It first examines CART (Classification and Regression Trees) and its strengths and weaknesses. The proposal is to use polar coordinates, which are more consistent with the basketball court geometry, and overcome CART's drawbacks by resorting to CART-based ensemble learning algorithms like Random Forest and Extremely Randomized Trees.
The query also defines an index to measure the map's graphical goodness, which can be used jointly with measures of out-of-sample error to tune the algorithm's parameters. The functioning of the proposed approaches is demonstrated through the analysis of real data from the NBA regular season 2020/2021.