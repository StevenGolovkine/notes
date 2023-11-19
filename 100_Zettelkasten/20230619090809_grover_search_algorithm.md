
---
creation date: 2023-06-19 09:07
last updated: 2023-06-19 09:07
---
# [[20230619090809_grover_search_algorithm]] - Grover's search algorithm
__Tags__: #quantum #algorithm-theory  

---
__Contents__: The Grover's algorithm is an algorithm that checks if a proposed solution is actually a solution of the problem.

The idea of the algorithm is to change the phase of the output state by $\pi$ if the state is a solution of the problem. For a state $\lvert x \rangle$,
$$U_{oracle}\lvert x \rangle = 
\left\{
	\begin{array}{r c l} 
		\lvert x \rangle &\text{if}& x \text{ is not a solution}\\  
		-\lvert x \rangle &\text{if}& x \text{ is a solution}\\  
	\end{array}  
\right.
$$
_Algortihm_:
1. Create an equal superposition of every possible input to the oracle. If all input start at $\lvert 0 \rangle$, apply a H-gate to each of them to create superposition. It results in state $\lvert s \rangle$.
2. Run the oracle on the qubits.
3. Run a circuit "diffusion operator", also named "diffuser". It is the same for every oracle.

Let $\lvert \checkmark \rangle$ be a solution state to the problem and $\lvert \mathsf{X} \rangle$ be a non-solution state to the problem. The Grover's algorithm has a geometrical interpertation (see Figure). The first step, passing through the oracle, is a reflection over $\lvert \mathsf{X} \rangle$, and the second step, running the diffuser, as a reflection over $\lvert s \rangle$. 

![[grover_algo.png]]

The oracle transforms $a\lvert \mathsf{X} \rangle + b\lvert \checkmark \rangle$ to $a\lvert \mathsf{X} \rangle - b\lvert \checkmark \rangle$. The diffuser transforms $\lvert s \rangle$ to $\lvert 11 \rangle$, then reflect around $\lvert 11 \rangle$ using a CNOT-gate, and finally retransform $\lvert 11 \rangle$ to $\lvert s \rangle$. Noting $\theta$ the angle between $\lvert s \rangle$ and $\lvert \mathsf{X} \rangle$, at each step, $\lvert s \rangle$ rotates of $2\theta$.

Assume there is only one solution to the problem. Then $\lvert s \rangle$ can be decompose as
$$\lvert s \rangle = \frac{1}{\sqrt{N}}\left(\lvert 0 \rangle + \lvert 1 \rangle + \dots + \lvert \checkmark \rangle + \dots + \lvert N - 1 \rangle\right).$$
Using basic trigonometry, $\sin \theta = \frac{1}{\sqrt{N}}$. For small $\theta$, $\sin \theta \approx \theta$. To reach $\pi / 2$, we need $\frac{\pi}{2 \times 2 \theta} = \frac{\pi}{4}\sqrt{N}$ steps. The number of steps to prove that a proposal is a solution to the problem is proportional to $\sqrt{N}$.

__References__:



