
---
creation date: 2023-03-13 11:48
last updated: 2023-03-13 11:48
---
# [[20230313114851_example_breakage_mixing]] - Example of breakage equation with Markov chain for particulate mixing problems

__Tags__: #breakage-equation #markov-chains #application 

---
__Contents__: It aims to describe variation with time of a property of particles. To do this estimation, the total duration of the process is divided into finite intervals of time $\Delta t$. The unidimensional MC can be extended to $n$-dimensional MC, i.e., $n$ properties studied simultaneously. The modeling of transition probabilities is process specific, from experimental data or theoretical model.

The structure of MC is different for each process:
* Motion of particles: transition matrix is tridiagonal with an absorbing state at the end.
* Batch mixing: No absorbing state and no feed vector
* Classification: Randomly feed in a middle state and absorbing states at the beginning and end states.
* Grinding: The probabilities to go to higher states is nul.
* Complex milling circuits: Combination of the above.
* Agglomeration: The transistion probabilities above the main diagonal are not nul.

**Questions**:
* Could it be extended to continuous state Markov chain?
* Could we use statistical model to estimate the transition probabilities matrix from data?

__References__:
[[@berthiauxApplicationTheoryMarkov2005]] - Berthiaux, Mizonov, Zhukov - _Application of the theory of Markov chains to model different processes in particle technology_ (2005)
