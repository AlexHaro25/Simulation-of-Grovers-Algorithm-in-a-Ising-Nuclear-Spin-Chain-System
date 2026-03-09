# Simulation of Grover's Algorithm in an Ising Nuclear Spin Chain System

## Description
This project presents a numerical simulation of Grover's quantum search algorithm for two qubits, using a one-dimensional Ising nuclear spin chain as the physical model. The system interacts with an external magnetic field and radiofrequency pulses, which are used to implement the required quantum gates. A reference simulation was also implemented using Qiskit.

## Quantum Gates Implemented
- Hadamard gate ($H_0$, $H_1$)
- Control-Z gate (CZ)
- $Z_1Z_2$ gate

## Physical Model
The system is based on a chain of $n$ nuclear spins (qubits) described by an Ising Hamiltonian, where quantum gates are implemented through radiofrequency pulses. The $2\pi k$ method is used to find the optimal Rabi frequency and suppress errors from non-resonant transitions.

## Decoherence Analysis
Two decoherence models were analyzed:
- **Case A — Independent Damping**: destroys quantum superposition by amplifying ground state probabilities
- **Case B — Pure Dephasing**: drives the system toward a maximally mixed state, making all states equally probable

## Key Results
- Grover's algorithm was successfully simulated for two qubits
- The $2\pi k$ method effectively suppresses non-resonant transition errors
- Independent damping has the greatest impact on algorithm fidelity
- Pure dephasing limits the algorithm for all possible search cases

## Libraries
- numpy
- scipy
- matplotlib
- qiskit

## Reference
Based on the Ising spin chain model for quantum computing as described in Berman et al. (2000) and Nielsen & Chuang (2010).
