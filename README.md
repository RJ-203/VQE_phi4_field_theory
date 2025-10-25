# VQE_phi4_field_theory
This project implements a Variational Quantum Eigensolver (VQE) to approximate the ground-state energy of a discretized ϕ⁴ scalar field theory — a fundamental model in quantum field theory. The simulation builds the Hamiltonian, embeds it into qubit space, and optimizes a quantum circuit using PennyLane to compare quantum and exact energies.

The algorithm followed is:
- A lattice ϕ⁴ Hamiltonian is constructed from creation and annihilation operators
- With a physical-state projector, binary qubit embedding is achieved
- A penalty term is added to enforce valid (physical) subspace
- Hamiltonian is deomposed into Pauli operators for VQE
- PennyLane-based VQE is run using StronglyEntanglingLayers ansatz
- Energy convergence and log-scale error reduction is plotted
