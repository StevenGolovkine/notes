
---
creation date: 2023-03-13 10:14
last updated: 2023-03-13 10:14
---
# [[20230313101418_abstract_population_balance]] - Abstraction of population balance models

__Tags__: #population-balance 

---
__Contents__: A set of particles can be view as an ensemble of systems of states. These systems of states contain:
* Internal coordinates (properties of the particles), e.g. number, mass, ...
* External coordinates (physical location of the center of mass of the particles)

Population balances are described by a quantitative (number, mass, ...) distribution of the particles in the joint space of internal and external coordinates. The internal coordinates can be either discrete or continuous, while external coordinates are usually continuous.
For example, for continuous internal coordinates, the size of the particles belongs to $\mathbb{R}$, while for discrete internal coordinates, particle sizes are discretized in bins (in that case, we assume that the process jumps from one state to another). 

**Questions**:
* Could we use the LASSO as a regularization strategy to be robust to errors in input data  in scaling behaviors?

__References__:
[[@ramkrishnaPopulationBalanceModeling2014]] - Ramkrishna and Singh - *Population Balance Modeling: Current Status and Future Prospects* (2014)