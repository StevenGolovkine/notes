
---
creation date: 2023-03-27 16:54
last updated: 2023-03-27 16:54
---
# [[20230327165411_model_based_clustering_functional_data]] - Model based clustering for functional data
__Tags__: #functional-data #clustering #model-based-clustering 

---
__Contents__: Model-based clustering algorithm for functional data is based on the truncation of the KL expansion. Usually, the coefficients are assumed to be Gaussian.

A mixture model for functional data is a surrogate based on the coefficients. The estimation of the parameters of the model (labels of the observations, center of the clusters) is performed by an EM algorithm ([[20230328105102_expectation_maximisation_algorithm]]).

_E-step_: Compute the conditional expectation of the likelihood.
* Update the probabilities of a curve to belong to each cluster
* Update the principal scores
* Estimate the approximation order (the number of retain components)
_M-step_: Update the mixture parameters that maximises the likelihood.

__References__:
[[@jacquesModelbasedClusteringMultivariate2014a]] - Jacques and Preda - _Model-based clustering for multivariate functional data_ (2014)