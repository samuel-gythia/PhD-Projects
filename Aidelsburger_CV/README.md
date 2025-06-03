# Continuous Variable Quantum Optics Simulation

This simulation demonstrates squeezed vacuum dynamics and continuous variable cluster states, inspired by the research of Prof. Monika Aidelsburger on quantum simulation with ultracold atoms and engineered gauge fields.

## Scientific Background

Continuous variable quantum optics explores quantum states with continuous eigenvalue spectra. This simulation focuses on:

- Single-mode and two-mode squeezing operations that reduce uncertainty in selected quadratures
- Generation of CV cluster states as a resource for measurement-based quantum computing
- Visualization of non-classical features through phase-space representations
- Applications to quantum simulation with engineered gauge fields

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

## References

Aidelsburger, M., et al. "Artificial gauge fields with ultracold atoms," *Rep. Prog. Phys.* **81**, 064401 (2018).  
[DOI:10.1088/1361-6455/aac120](https://doi.org/10.1088/1361-6455/aac120)

## How to Run

```bash
conda activate qc-env
jupyter lab
```