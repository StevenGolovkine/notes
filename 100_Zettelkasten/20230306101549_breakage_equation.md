
---
creation date: 2023-03-06 10:15
last updated: 2023-03-13 11:00
---
# [[20230306101549_breakage_equation]] - Breakage equation 

__Tags__: #breakage-equation 

---
__Contents__: Breakage equation is used to model the fragmentation of particles process. The equation is given by
$$\frac{dn(t, u)}{dt} = \int_{u}^{\infty} b^\prime(u, w)S(w)n(w, t) \mathrm{d}w - S(u)n(u, t),$$
where the variable $t$ refers to time and the variables $u$ and $w$ are particle volumes.
The function $n$ is the distribution of the number of particles. The function $b^\prime$ is the breakage distribution function (usually not symetric). The function $S$ is the rate of breakage that depends on the mass of the particle.
Experimental data of the particle size distribution (PSD) can be obtained at various times as the breakage process progress.

Breakage equations can be modelled by a Markov chain ([[20230313110112_markov_chain_for_breakage]]).

**Questions**:
* Would it be possible to infer the particle type from observed data?
* Can we deternine the functional form of $b^\prime$ from experimental data on the particle-size distribution (PSD)?

__References__:
[[@hillStatisticsMultipleParticle1996]] - Hill and Ng - _Statistics of Multiple Particle Breakage_ (1996)


