---
category: readingnote
File: "[[cervoneMultiresolutionStochasticProcess2016]]"
itemType: note
Status: unread
Date first pass: 24/10/2024
Date second pass: 
Date third pass: 
Clarity: ⭐️⭐️⭐️
Rank: ⭐️⭐️⭐️⭐️⭐️
Figure to add: 
VUE do: false
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
A multiresolution stochastic process model for predicting basketball outcomes

# Learning goal (why read this?)
Learn about the analysis of basketball games

# Task or problem (what are they solving?)
Estimation of the expected number of points obtained by the end of a possession

# Data and domain (with what and where?)
Optical player tracking data

# Context and relationship (new approach, specialisation of, generalisation of, application of, survey of, example of, ...)
New approach to model the dynamics of the game.

# Summary and contributions

Basketball games are complex systems that evolve over time as players interact with each other, their teammates, opponents, and the ball. Current analyses of basketball outcomes rely on discrete summaries of the game, such as points scored, assists made, etc. However, a more nuanced approach is needed to understand the dynamics of the game.

To address this, researchers propose a framework for estimating the expected number of points obtained by the end of a possession (EPV) using optical player tracking data. This framework uses a stochastic process model that captures both continuous and discrete events in the game.

The model is based on hierarchical spatiotemporal models that share information across players while remaining computationally tractable even with large datasets. In addition to estimating EPV, these models reveal insights into players' decision-making tendencies as a function of their spatial strategy.