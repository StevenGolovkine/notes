
---
creation date: 2023-04-26 10:20
last updated: 2023-04-26 10:20
---
# [[20230426102011_probability_amplitudes]] - Probability amplitudes
__Tags__: #quantum

---
__Contents__: Probability amplitudes are tools to describe quantum mechanics. This is a probability with an extra property: the phase (which correspond to a direction).
In that case, probability amplitudes are represented as complex numbers:
$$p = a + b\mathbf{i},$$
where $a$ is the magnitude and $b$ is the phase. We use state vectors ([[20230426104728_state_vectors]]) to keep track of the amplitudes of all possible outcomes (and thus, it is possible to use linear algebra to derive quantities of interest). Pay attention that for $n$ qubits, we need to keep track of $2^n$ amplitudes.

The probability of measuring an outcome is the square of the magnitude of the outcome's amplitude. An important property of the amplitudes are the **interference**: two amplitudes with the same magnitude and opposite phase cancel each others. It is like they look at opposite direction with the same strengh. 

For the H-gate:
* If the input is $\left|0\right>$, the H-gate will output $\left|0\right>$ with probability $1/2$ and $\left|1\right>$ with probabilty $1/2$ and the direction will be the same.
* If the input is $\left|1\right>$, the H-gate will output $\left|0\right>$ with probability $1/2$ and $\left|1\right>$ with probabilty $1/2$ and the direction will swap for $\left| 1\right>$.

How gates transform amplitudes:
* X-gate swaps the amplitudes and keep the directions.
* Y-gate swaps the amplitudes and reverse the direction of $\left| 1 \right>$.
* Z-gate does not swap the amplitudes but reverse the direction of $\left| 1\right>$.

__References__:


