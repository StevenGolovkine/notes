
---
creation date: 2023-04-26 11:02
last updated: 2023-04-26 11:02
---
# [[20230426110222_quantum_operations]] - Quantum operations
__Tags__: #quantum 

---
__Contents__: Quantum operations (going through gates) are represented using matrices.

For two qubits, we note this matrice
$$U = \left[ t_{ij \rightarrow i^\prime j^\prime}\right], \quad i, j, i^\prime, j^\prime \in \{0, 1\}.$$
For example, for the CNOT-gate, we have
$$CNOT = \begin{pmatrix} 1 & 0 & 0 & 0 \\ 0 & 0 & 0 & 1 \\ 0 & 0 & 1 & 0 \\ 0 & 1 & 0 & 0 \end{pmatrix}.$$
To look for the effect of a gate onto a qubit, we use matrix multiplication.

$$H \left| 0 \right> = \frac{1}{\sqrt{2}} \begin{pmatrix} 1 & 1 \\ 1 & -1 \end{pmatrix}\begin{pmatrix} 1 \\ 0\end{pmatrix} = \frac{1}{\sqrt{2}} \begin{pmatrix} 1 \\ 1\end{pmatrix}$$
$$H \left| 1 \right> = \frac{1}{\sqrt{2}} \begin{pmatrix} 1 & 1 \\ 1 & -1 \end{pmatrix}\begin{pmatrix} 0 \\ 1\end{pmatrix} = \frac{1}{\sqrt{2}} \begin{pmatrix} 1 \\ -1\end{pmatrix}$$

Every unitary matrice is a valid quantum operation because it keeps the total output probabilities equal to $1$.

__References__:

