
---
creation date: 2023-06-06 10:48
last updated: 2023-06-06 10:48
---
# [[20230606104817_bells_inequalities]] - Bell's inequalities
__Tags__: #quantum 

---
__Contents__: Let $A$ and $B$ two variables. A hash function takes an input variable and return an output bit. Note $H$ and $V$ two hashing types.

For usual bits: $\mathbb{P}(H)$ is the probability that a variable is set to $1$ after the hashing function $H$ and $\mathbb{P}(HV)$ is the probability that $A$ is $1$ after $H$ and $B$ is $0$ after $V$ or $A$ is $0$ after $H$ and $B$ is $1$ after $V$ ($A$ and $B$ disagree).

Bell's inequalities:
$$\mathbb{P}(HH) \leq \mathbb{P}(HV) + \mathbb{P}(VH) + \mathbb{P}(VV)$$
$$\mathbb{P}(HV) \leq \mathbb{P}(HH) + \mathbb{P}(VH) + \mathbb{P}(VV)$$
$$\mathbb{P}(VH) \leq \mathbb{P}(HV) + \mathbb{P}(HH) + \mathbb{P}(VV)$$
$$\mathbb{P}(VV) \leq \mathbb{P}(HV) + \mathbb{P}(VH) + \mathbb{P}(HH)$$

For qubits, we use z-measurement as $V$ type hash and x-measurement as $H$ type hash. Bell's inequalities do not apply to qubits because the result of hash is not known before we do it and the result of one hash depends on the result of the other.

__References__:
