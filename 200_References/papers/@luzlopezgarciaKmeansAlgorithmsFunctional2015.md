---
category: literaturenote
tags:
  - clustering
  - dimension-reduction
  - functional-data-analysis
  - reproducing-kernel-hilbert-space
citekey: luzlopezgarciaKmeansAlgorithmsFunctional2015
itemType: journalArticle
status: read
dateread: 2023/11/06
---

> [!Cite]  
> Luz López García, María, Ricardo García-Ródenas, and Antonia González Gómez. 2015. “K-Means Algorithms for Functional Data.” _Neurocomputing_ 151 (March): 231–45. [https://doi.org/10.1016/j.neucom.2014.09.048](https://doi.org/10.1016/j.neucom.2014.09.048).

> [!SYNTHESIS] 
>**Contribution**::
>
>**Related**:: 
>

> [!METADATA]  
>
**Author**:: Luz López García, María
**Author**:: García-Ródenas, Ricardo
**Author**:: González Gómez, Antonia<br>
> **Title**:: K-means algorithms for functional data    
> **Year**:: 2015     
> **Citekey**:: @luzlopezgarciaKmeansAlgorithmsFunctional2015    
>**Journal**:: *Neurocomputing*    
>**Volume**:: 151    
>     
>    
>    
>     
> **Pages**:: 231-245    
>**DOI**:: 10.1016/j.neucom.2014.09.048    
>
>**Smoothing**:: RKHS

> [!LINK] 
>
> [Luz López García et al_2015_K-means algorithms for functional data.pdf](file:///Users/steven/Library/CloudStorage/GoogleDrive-steven.golovkine@ul.ie/My%20Drive/bibliography/Neurocomputing/2015/Luz%20López%20García%20et%20al_2015_K-means%20algorithms%20for%20functional%20data.pdf).

>[!Abstract]
>
>Cluster analysis of functional data considers that the objects on which you want to perform a taxonomy are functions f:X⊂Rp↦R and the available information about each object is a sample in a finite set of points fn={(xi,yi)∈X×R}i=1n. The aim is to infer the meaningful groups by working explicitly with its infinite-dimensional nature. In this paper the use of K-means algorithms to solve this problem is analysed. A comparative study of three K-means algorithms has been conducted. The K-means algorithm for raw data, a kernel K-means algorithm for raw data and a K-means algorithm using two distances for functional data are tested. These distances, called dVn and dϕ, are based on projections onto Reproducing Kernel Hilbert Spaces (RKHS) and Tikhonov regularization theory. Although it is shown that both distances are equivalent, they lead to two different strategies to reduce the dimensionality of the data. In the case of dVn distance the most suitable strategy is Johnson–Lindenstrauss random projections. The dimensionality reduction for dϕ is based on spectral methods. A key aspect that has been analysed is the effect of the sampling {xi}i=1n on the K-means algorithm performance. In the numerical study an ex professo example is given to show that if the sampling is not uniform in X, then a K-means algorithm that ignores the functional nature of the data can reduce its performance. It is numerically shown that the original K-means algorithm and that suggested here lead to similar performance in the examples when X is uniformly sampled, but the computational cost when working with the original set of observations is higher than the K-means algorithms based on dϕ or dVn, as they use strategies to reduce the dimensionality of the data. The numerical tests are completed with a case study to analyse what kind of problem the K-means algorithm for functional data must face.
>>


# Notes<br>
# Annotations%% begin annotations %%  
 
  
  
 
 
  
### Imported: 2023-10-31 2:35 pm  
  
  
<mark style="background-color: #f9cd59">Quote</mark>  
> a point in a general function space and then project these points onto a Reproducing Kernel Hilbert Space (RKHS) by using the Tikhonov regularization theory.
  
<mark style="background-color: #f9cd59">Quote</mark>  
> The method proposed in this paper is an instance of a two-stage method but it allows the algorithms of this class to be reinterpreted (mainly based on it functional principal component analysis) as methods that compute the similarity measure as the distance between the projections of the data onto a Hilbert space.
  
<mark style="background-color: #f9cd59">Quote</mark>  
> The proposed algorithm, named KK-means, consists of applying the K-means algorithm to functional data using projections on RKHS.
  
  
%% end annotations %%

%% Import Date: 2023-10-31T14:35:25.858+00:00 %%
