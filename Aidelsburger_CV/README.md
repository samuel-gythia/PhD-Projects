# Continuous Variable Quantum Optics Simulation

This simulation demonstrates squeezed vacuum dynamics and continuous variable cluster states, visualizing the quantum mechanical properties through Wigner functions.

## Scientific Background

Continuous variable quantum optics explores quantum states with continuous eigenvalue spectra. This simulation focuses on:

- Single-mode and two-mode squeezing operations that reduce uncertainty in selected quadratures
- Generation of CV cluster states as a resource for measurement-based quantum computing
- Visualization of non-classical features through phase-space representations

## Implementation Details

The simulation uses QuTiP to model:

1. Single-mode squeezing under Hamiltonian H = i r (a†² − a²)
   - Tracks variance in X/P quadratures over time
   - Demonstrates uncertainty principle as one quadrature is squeezed

2. Two-mode squeezing under Hamiltonian H = i r (a†b† − ab)
   - Creates entanglement between modes
   - Shows correlated/anti-correlated quadrature variances

3. CV Cluster state preparation
   - Applies S(r) squeezing operation on each mode
   - Implements CZ = exp(i g X₁X₂) operation
   - Computes Wigner functions to visualize quantum features

## Performance Metrics

- **Single-Mode Squeezing:**
  ![single_mode_squeezing](single_mode_squeezing.png)

- **Two-Mode Squeezing:**
  ![two_mode_squeezing](two_mode_squeezing.png)

- **CV Cluster State Wigner Functions:**
  ![wigner_cluster_modes](wigner_cluster_modes.png)

## How to Run

```bash
conda activate qc-env
jupyter lab
```