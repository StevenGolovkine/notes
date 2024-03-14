---
category: literaturenote
tags: deep-learning, functional-principal-components, neural-network, uncertainty-quantification
citekey: xieFunctionalPCADeep2023
itemType: preprint
status: unread  
dateread:  
---

> [!Cite]  
> Xie, Ziyu, Mahmoud Yaseen, and Xu Wu. 2023. “Functional PCA and Deep Neural Networks-Based Bayesian Inverse Uncertainty Quantification with Transient Experimental Data.” arXiv. [https://doi.org/10.48550/arXiv.2307.05592](https://doi.org/10.48550/arXiv.2307.05592).

> [!SYNTHESIS] 
>**Contribution**::
>
>**Related**:: 
>

> [!METADATA]  
>
**Author**:: Xie, Ziyu
**Author**:: Yaseen, Mahmoud
**Author**:: Wu, Xu<br>
> **Title**:: Functional PCA and Deep Neural Networks-based Bayesian Inverse Uncertainty Quantification with Transient Experimental Data    
> **Year**:: 2023     
> **Citekey**:: @xieFunctionalPCADeep2023    
>    
>    
>     
>    
>    
>     
>    
>**DOI**:: 10.48550/arXiv.2307.05592    
>
>**Smoothing**:: FPCA

> [!LINK] 
>
> [Xie et al_2023_Functional PCA and Deep Neural Networks-based Bayesian Inverse Uncertainty.pdf](file:///Users/steven/Library/CloudStorage/GoogleDrive-steven.golovkine@ul.ie/My%20Drive/bibliography/arXiv/2023/Xie%20et%20al_2023_Functional%20PCA%20and%20Deep%20Neural%20Networks-based%20Bayesian%20Inverse%20Uncertainty.pdf).

>[!Abstract]
>
>Inverse UQ is the process to inversely quantify the model input uncertainties based on experimental data. This work focuses on developing an inverse UQ process for time-dependent responses, using dimensionality reduction by functional principal component analysis (PCA) and deep neural network (DNN)-based surrogate models. The demonstration is based on the inverse UQ of TRACE physical model parameters using the FEBA transient experimental data. The measurement data is time-dependent peak cladding temperature (PCT). Since the quantity-of-interest (QoI) is time-dependent that corresponds to infinite-dimensional responses, PCA is used to reduce the QoI dimension while preserving the transient profile of the PCT, in order to make the inverse UQ process more efficient. However, conventional PCA applied directly to the PCT time series profiles can hardly represent the data precisely due to the sudden temperature drop at the time of quenching. As a result, a functional alignment method is used to separate the phase and amplitude information of the transient PCT profiles before dimensionality reduction. DNNs are then trained using PC scores from functional PCA to build surrogate models of TRACE in order to reduce the computational cost in Markov Chain Monte Carlo sampling. Bayesian neural networks are used to estimate the uncertainties of DNN surrogate model predictions. In this study, we compared four different inverse UQ processes with different dimensionality reduction methods and surrogate models. The proposed approach shows an improvement in reducing the dimension of the TRACE transient simulations, and the forward propagation of inverse UQ results has a better agreement with the experimental data.
>>


# Notes
Comment: 31 pages, 21 figures<br>
# Annotations%% begin annotations %%  
 
  
%% end annotations %%

%% Import Date: 2023-10-27T13:12:54.227+01:00 %%
