---
category: literaturenote
tags: ecology, random-fields, stochastic-differential-equation
citekey: camelettiSpatiotemporalModelingParticulate2013
itemType: journalArticle
status: unread  
dateread:  
---

> [!Cite]  
> Cameletti, Michela, Finn Lindgren, Daniel Simpson, and Håvard Rue. 2013. “Spatio-Temporal Modeling of Particulate Matter Concentration through the SPDE Approach.” _AStA Advances in Statistical Analysis_ 97 (2): 109–31. [https://doi.org/10.1007/s10182-012-0196-3](https://doi.org/10.1007/s10182-012-0196-3).

> [!SYNTHESIS] 
>**Contribution**::
>
>**Related**:: 
>

> [!METADATA]  
>
**Author**:: Cameletti, Michela
**Author**:: Lindgren, Finn
**Author**:: Simpson, Daniel
**Author**:: Rue, Håvard<br>
> **Title**:: Spatio-temporal modeling of particulate matter concentration through the SPDE approach    
> **Year**:: 2013     
> **Citekey**:: @camelettiSpatiotemporalModelingParticulate2013    
>**Journal**:: *AStA Advances in Statistical Analysis*    
>**Volume**:: 97    
>**Issue**:: 2     
>    
>    
>     
> **Pages**:: 109-131    
>**DOI**:: 10.1007/s10182-012-0196-3    
>

> [!LINK] 
>
> [Cameletti et al_2013_Spatio-temporal modeling of particulate matter concentration through the SPDE.pdf](file:///Users/steven/Library/CloudStorage/GoogleDrive-steven.golovkine@ul.ie/My%20Drive/bibliography/AStA%20Advances%20in%20Statistical%20Analysis/2013/Cameletti%20et%20al_2013_Spatio-temporal%20modeling%20of%20particulate%20matter%20concentration%20through%20the%20SPDE.pdf).

>[!Abstract]
>
>In this work, we consider a hierarchical spatio-temporal model for particulate matter (PM) concentration in the North-Italian region Piemonte. The model involves a Gaussian Field (GF), affected by a measurement error, and a state process characterized by a first order autoregressive dynamic model and spatially correlated innovations. This kind of model is well discussed and widely used in the air quality literature thanks to its flexibility in modelling the effect of relevant covariates (i.e. meteorological and geographical variables) as well as time and space dependence. However, Bayesian inference—through Markov chain Monte Carlo (MCMC) techniques—can be a challenge due to convergence problems and heavy computational loads. In particular, the computational issue refers to the infeasibility of linear algebra operations involving the big dense covariance matrices which occur when large spatio-temporal datasets are present. The main goal of this work is to present an effective estimating and spatial prediction strategy for the considered spatio-temporal model. This proposal consists in representing a GF with Matérn covariance function as a Gaussian Markov Random Field (GMRF) through the Stochastic Partial Differential Equations (SPDE) approach. The main advantage of moving from a GF to a GMRF stems from the good computational properties that the latter enjoys. In fact, GMRFs are defined by sparse matrices that allow for computationally effective numerical methods. Moreover, when dealing with Bayesian inference for GMRFs, it is possible to adopt the Integrated Nested Laplace Approximation (INLA) algorithm as an alternative to MCMC methods giving rise to additional computational advantages. The implementation of the SPDE approach through the R-library INLA (www.r-inla.org) is illustrated with reference to the Piemonte PM data. In particular, providing the step-by-step R-code, we show how it is easy to get prediction and probability of exceedance maps in a reasonable computing time.
>>


# Notes<br>
# Annotations%% begin annotations %%  
 
  
%% end annotations %%

%% Import Date: 2023-10-24T12:04:37.725+01:00 %%
