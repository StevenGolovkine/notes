---
category: literaturenote
tags: physics-informed-model, differential-equation, gaussian-process, operator-theory
citekey: pfortnerPhysicsInformedGaussianProcess2023
itemType: preprint
status: unread  
dateread:  
---

> [!Cite]  
> Pförtner, Marvin, Ingo Steinwart, Philipp Hennig, and Jonathan Wenger. 2023. “Physics-Informed Gaussian Process Regression Generalizes Linear PDE Solvers.” arXiv. [https://doi.org/10.48550/arXiv.2212.12474](https://doi.org/10.48550/arXiv.2212.12474).

> [!SYNTHESIS] 
>**Contribution**::
>
>**Related**:: 
>

> [!METADATA]  
>
**Author**:: Pförtner, Marvin
**Author**:: Steinwart, Ingo
**Author**:: Hennig, Philipp
**Author**:: Wenger, Jonathan<br>
> **Title**:: Physics-Informed Gaussian Process Regression Generalizes Linear PDE Solvers    
> **Year**:: 2023     
> **Citekey**:: @pfortnerPhysicsInformedGaussianProcess2023    
>    
>    
>     
>    
>    
>     
>    
>**DOI**:: 10.48550/arXiv.2212.12474    
>

> [!LINK] 
>
> [Pförtner et al_2023_Physics-Informed Gaussian Process Regression Generalizes Linear PDE Solvers.pdf](file:///Users/steven/Library/CloudStorage/GoogleDrive-steven.golovkine@ul.ie/My%20Drive/bibliography/arXiv/2023/Pförtner%20et%20al_2023_Physics-Informed%20Gaussian%20Process%20Regression%20Generalizes%20Linear%20PDE%20Solvers.pdf).

>[!Abstract]
>
>Linear partial differential equations (PDEs) are an important, widely applied class of mechanistic models, describing physical processes such as heat transfer, electromagnetism, and wave propagation. In practice, specialized numerical methods based on discretization are used to solve PDEs. They generally use an estimate of the unknown model parameters and, if available, physical measurements for initialization. Such solvers are often embedded into larger scientific models with a downstream application and thus error quantification plays a key role. However, by ignoring parameter and measurement uncertainty, classical PDE solvers may fail to produce consistent estimates of their inherent approximation error. In this work, we approach this problem in a principled fashion by interpreting solving linear PDEs as physics-informed Gaussian process (GP) regression. Our framework is based on a key generalization of the Gaussian process inference theorem to observations made via an arbitrary bounded linear operator. Crucially, this probabilistic viewpoint allows to (1) quantify the inherent discretization error; (2) propagate uncertainty about the model parameters to the solution; and (3) condition on noisy measurements. Demonstrating the strength of this formulation, we prove that it strictly generalizes methods of weighted residuals, a central class of PDE solvers including collocation, finite volume, pseudospectral, and (generalized) Galerkin methods such as finite element and spectral methods. This class can thus be directly equipped with a structured error estimate. In summary, our results enable the seamless integration of mechanistic models as modular building blocks into probabilistic models by blurring the boundaries between numerical analysis and Bayesian inference.
>>


# Notes<br>
# Annotations%% begin annotations %%  
 
  
%% end annotations %%

%% Import Date: 2023-10-24T12:09:06.930+01:00 %%
