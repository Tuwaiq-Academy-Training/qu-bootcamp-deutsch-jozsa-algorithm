# qu-bootcamp-deutsch-jozsa algorithm

## Introduction

The Deutsch-Jozsa algorithm is one of the earliest quantum algorithms that shows a quantum computer's advantage over classical computers. It aims to solve the "black-box" problem, where we are given a function, and we need to determine whether the function is constant or balanced.

In the classical world, to find this answer for a given function f, we would need to evaluate f(x) for half of all possible inputs to determine if the function is constant or not. However, with the Deutsch-Jozsa algorithm, we can solve this problem with just one function evaluation, making it exponentially faster than the classical approach.

## Oracle

In the Deutsch-Jozsa algorithm, we use an oracle that implements the function f as a quantum operator. The oracle takes two quantum registers: the first register contains the input qubits, and the second register contains the output qubit. The oracle performs the following transformation:

1. If f(x) is constant (returns the same value for all inputs x), the oracle applies an identity transformation to the output qubit.

2. If f(x) is balanced (returns different values for exactly half of the inputs x), the oracle applies a NOT gate (X gate) to the output qubit.
       
![deutsch-jozsa algorithm Oracle](https://upload.wikimedia.org/wikipedia/commons/b/b5/Deutsch-Jozsa-algorithm-quantum-circuit.png)
## Task

Using Qiskit, we will implement the Deutsch-Jozsa algorithm, where the user chooses the number of qubits and whether the oracle represents a constant or balanced function randomly.

## Output

The code will include the quantum circuit to perform the Deutsch-Jozsa algorithm on the randomly generated oracle, and it will display the result indicating whether the function is constant or balanced. Additionally, the code will include comments explaining each step of the algorithm and how the oracle is represented in the quantum circuit.




# References

> [Qiskit documentation](https://qiskit.org/documentation/)   
> [introduction to classical and quantum computing-book](https://www.thomaswong.net/introduction-to-classical-and-quantum-computing-1e3p.pdf)
