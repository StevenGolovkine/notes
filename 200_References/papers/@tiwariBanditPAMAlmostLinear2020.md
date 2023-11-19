---
category: literaturenote
tags: bandits-theory, clustering, python-software
citekey: tiwariBanditPAMAlmostLinear2020
itemType: conferencePaper
status: unread  
dateread:  
---

> [!Cite]  
> Tiwari, Mo, Martin J Zhang, James Mayclin, Sebastian Thrun, Chris Piech, and Ilan Shomorony. 2020. “BanditPAM: Almost Linear Time k-Medoids Clustering via Multi-Armed Bandits.” In _Advances in Neural Information Processing Systems_, 33:10211–22. Curran Associates, Inc. [https://proceedings.neurips.cc/paper_files/paper/2020/hash/73b817090081cef1bca77232f4532c5d-Abstract.html](https://proceedings.neurips.cc/paper_files/paper/2020/hash/73b817090081cef1bca77232f4532c5d-Abstract.html).

> [!SYNTHESIS] 
>**Contribution**::
>
>**Related**:: 
>

> [!METADATA]  
>
**Author**:: Tiwari, Mo
**Author**:: Zhang, Martin J
**Author**:: Mayclin, James
**Author**:: Thrun, Sebastian
**Author**:: Piech, Chris
**Author**:: Shomorony, Ilan<br>
> **Title**:: BanditPAM: Almost Linear Time k-Medoids Clustering via Multi-Armed Bandits    
> **Year**:: 2020     
> **Citekey**:: @tiwariBanditPAMAlmostLinear2020    
>    
>**Volume**:: 33    
>     
>    
>**Publisher**:: Curran Associates, Inc.    
>     
> **Pages**:: 10211–10222    
>    
>

> [!LINK] 
>
> [Tiwari et al_2020_BanditPAM.pdf](file:///Users/steven/Library/CloudStorage/GoogleDrive-steven.golovkine@ul.ie/My%20Drive/bibliography/Curran%20Associates,%20Inc./2020/Tiwari%20et%20al_2020_BanditPAM.pdf).

>[!Abstract]
>
>Clustering is a ubiquitous task in data science. Compared to the commonly used k-means clustering, k-medoids clustering requires the cluster centers to be actual data points and supports arbitrary distance metrics, which permits greater interpretability and the clustering of structured objects. Current state-of-the-art k-medoids clustering algorithms, such as Partitioning Around Medoids (PAM), are iterative and are quadratic in the dataset size n for each iteration, being prohibitively expensive for large datasets. We propose BanditPAM, a randomized algorithm inspired by techniques from multi-armed bandits, that reduces the complexity of each PAM iteration from O(n^2) to O(nlogn) and returns the same results with high probability, under assumptions on the data that often hold in practice. As such, BanditPAM matches state-of-the-art clustering loss while reaching solutions much faster. We empirically validate our results on several large real-world datasets, including a coding exercise submissions dataset from Code.org, the 10x Genomics 68k PBMC single-cell RNA sequencing dataset, and the MNIST handwritten digits dataset. In these experiments, we observe that BanditPAM returns the same results as state-of-the-art PAM-like algorithms up to 4x faster while performing up to 200x fewer distance computations. The improvements demonstrated by BanditPAM enable k-medoids clustering on a wide range of applications, including identifying cell types in large-scale single-cell data and providing scalable feedback for students learning computer science online. We also release highly optimized Python and C++ implementations of our algorithm.
>>


# Notes<br>
# Annotations%% begin annotations %%  
 
  
%% end annotations %%

%% Import Date: 2023-10-24T10:33:03.750+01:00 %%
