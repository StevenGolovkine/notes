
---
creation date: 2023-03-27 16:21
last updated: 2023-03-27 16:21
---
# [[20230327162113_number_of_components]] - Estimation of the number of components for FPCA
__Tags__: #functional-data #functional-principal-components  

---
__Contents__: There is multiple way to estimate the number of components for FPCA.

In the multivariate functional data case, the number of components $K_p$ are selected for each individual components, and then we choose $K \leq \sum_p K_p$.

__Questions__: 
* Maybe, the estimation of the number of components for multivariate functional data is not reasonable, and only $K \leq \min_p K_p$ can be estimated.

__References__:
[[@happMultivariateFunctionalPrincipal2015]] - Happ and Greven - _Multivariate Functional Principal Component Analysis for Data Observed on Different (Dimensional) Domains_ (2015)
