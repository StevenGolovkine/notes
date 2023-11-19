
---
creation date: 2023-03-20 15:04
last updated: 2023-03-20 15:04
---
# [[20230320150412_regularized_fpca]] - Regularized FPCA
__Tags__: #functional-principal-components 

---
__Contents__: Regularized FPCA concerns the smoothing of the principal components itself.

* Penalization of the roughness of $\phi$ using its integrated squared second derivative over the interval of interest $|\!| D^2\phi |\!|$ .The idea is to penalize the sample variance by adding the constraint $\langle \phi_j, \phi_k\rangle + \langle D^2\phi_j, D^2\phi_k\rangle = 0$. The smoothness parameter can be evaluated by cross-validation based on the minimisation of the norm of the residuals. In practice, using a suitable basis, we can derive an expression for the penalty.
* Alternative approaches:
	* Direct smoothing of the curves (e.g. by roughness penalty)
	* By stepwise roughness penalty. The smoothing penalty is different for each eigenfunction.

__References__:
[[@ramsayFunctionalDataAnalysis2005]] - Ramsay and Silverman - _Functional Data Analysis_ (2005)


