
---
creation date: 2023-04-06 10:28
last updated: 2023-04-06 10:28
---
# [[20230406102827_spatial_decomposition_simulation]] - Spatial decomposition algorithm for fluid dynamics simultion
__Tags__: #population-balance #simulation 

---
__Contents__: In order to simulate computational fluid dynamics, a data-driven spatial decomposition algorithm with particle agglomerations has been proposed ([[@martinezrodriguezParticleAgglomerationFlows2022]]). It controls numerical errors caused by non-homogeneous concentrations of particles (non-uniformity). The D2SD algorithm detects the presence of non-uniformity of point particles and computes an optimal spatial decomposition (local uniformity). The found regions are then classified using the number density function. The density of the particles is estimated using something similar to kernel estimation and use "a battery" of statistical tests to determine uniformity (_looks like p-hacking_). The simulations are done by generating particles with respect to each cell.

__References__:
[[@martinezrodriguezParticleAgglomerationFlows2022]] - Martínez Rodríguez, Bossy, Henry - _Particle agglomeration in flows: Fast data-driven spatial decomposition algorithm for CFD simulations_ (2022)


