---
category: readingnote
File: "[[franksCharacterizingSpatialStructure2015]]"
itemType: note
Status: unread
Date first pass: 24/10/2024
Date second pass: 
Date third pass: 
Clarity: ⭐️⭐️⭐️⭐️
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
To be re-implement: false
Re-implemented: false
Write article: false
Done article: false
---
# Title of the paper
Characterizing the Spatial Structure of Defensive Skill in Professional Basketball

# Learning goal (why read this?)
Understand the application of stochastic processes to defense effectiveness

# Task or problem (what are they solving?)
Characterize the defensive effectiveness of players

# Data and domain (with what and where?)
Optical tracker data from the 2013-2014 NBA season

# Context and relationship (new approach, specialisation of, generalisation of, application of, survey of, example of, ...)
New approach to model defensive effectiveness.

# Summary and contributions

The article highlights the limitations of traditional defensive statistics in basketball, which are largely based on offensive metrics. Steals, blocks, and defensive rebounds provide only a limited summary of defensive effectiveness, leading to a qualitative state of defensive analytics that is prone to human biases and imprecision.
Emerging optical player tracking systems have the potential to enable a richer quantitative characterization of basketball performance, particularly defensive performance. However, this potential remains unmet due to computational and methodological complexities.
To address this void, the article proposes an approach that combines spatial and spatiotemporal processes, matrix factorization techniques, and hierarchical regression models with player tracking data. This approach aims to advance the state of defensive analytics in the NBA by detecting, characterizing, and quantifying multiple aspects of defensive play.
The results support some common understandings of defensive effectiveness, challenge others, and open up many new insights into the defensive elements of basketball.

- model shot selection and its expected outcome given the defensive assignment
- create a defensive shot chart
- model shot charts using log Gaussian Cox process and non-negative matrix factorization (same as [[millerFactorizedPointProcess2014]])
- define defender types using the fraction of time that each defender spends guarding a shooter in each of the bases (from the decomposition) and run a $k$-means on the "time-spent" matrix.
