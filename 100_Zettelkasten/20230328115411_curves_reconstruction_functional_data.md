
---
creation date: 2023-03-28 11:54
last updated: 2023-03-28 11:54
---
# [[20230328115411_curves_reconstruction_functional_data]] - Curves reconstruction of functional data
__Tags__: #functional-data 

---
__Contents__: 

**Smoothing first, then estimation** paradigm ([[@zhangStatisticalInferencesFunctional2007a]]) consists to reconstruct each curve individually first, and then estimate quantities of interest based on these new set of curves. A way to estimate individual curve is to use local polynomials ([[20230606101448_kernel_smoothing_methods]]) using GCV rule for bandwidth selection. The smooth curves can then be used to estimate mean, covariance and noise functions. As the curves are usually assumed to be generated from the same process, we should use the same bandwidth for smoothing all the curves (but estimate the bandwidth using all the curves) ([[20230612090712_bandwidth_estimation_fda]]). To make the measurement errors ignorable via LPK smoothing, the number of measurements (sampling points) of all subjects should tend to infinity slightly faster than the number of subjects.


* Asymptotic point-wise confidence intervals
* Simultaneous confidence bands


__References__:
[[@zhangStatisticalInferencesFunctional2007a]] - J.-T. Zhang, J. Chen - *Statistical inferences for functional data* (2007)
