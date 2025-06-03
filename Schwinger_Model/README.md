# Lattice Schwinger Model Simulation

This simulation demonstrates key phenomena in (1+1)D lattice quantum electrodynamics (QED) using exact diagonalization techniques to explore ground state properties and quench dynamics.

## Scientific Background

The Schwinger model is a (1+1)-dimensional quantum field theory that describes the interaction between fermions and U(1) gauge fields. This simulation explores:

- Quantum entanglement in the ground state as a function of fermion mass
- String-breaking phenomena in gauge theories
- Dynamical evolution after quantum quenches
- Confinement and deconfinement phases in gauge theories

## Implementation Details

The simulation uses exact diagonalization to solve small lattice systems:

1. Ground state entanglement analysis:
   - Constructs the Hamiltonian H(m) for 4 matter sites + 3 gauge links
   - Computes the ground state using sparse matrix diagonalization
   - Calculates von Neumann entropy of the left half of the system
   - Tracks how entanglement varies with fermion mass parameter

2. String-breaking quench dynamics:
   - Prepares an initial state with charges at the system boundaries
   - Performs a sudden quench of the mass parameter to m = 0.5
   - Evolves the system using the time-dependent Schrödinger equation
   - Tracks expectation values of matter density ⟨n⟩ and gauge field ⟨S_z⟩

## Performance Metrics

The simulation produces three key visualizations:

- **Ground State Entanglement vs. Mass:**
  ![entanglement_vs_mass](entanglement_vs_mass.png)
  
  Shows how quantum entanglement in the ground state varies with fermion mass

- **Matter Density After Quench:**
  ![quench_matter](quench_matter.png)
  
  Demonstrates the dynamics of charge density following a sudden quench

- **Gauge Field After Quench:**
  ![quench_gauge](quench_gauge.png)
  
  Visualizes the evolution of gauge field expectation values during string breaking

## How to Run

```bash
conda activate qc-env
jupyter lab
```