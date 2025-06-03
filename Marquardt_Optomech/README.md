# Cavity Optomechanics Cooling Simulation

This simulation reproduces core concepts from cavity optomechanics, focusing on sideband cooling of mechanical motion in different parameter regimes as pioneered in the work of Marquardt et al.

## Scientific Background

Cavity optomechanics studies the interaction between light and mechanical motion. This simulation explores:

- Cooling of mechanical oscillators using radiation pressure forces
- Comparison between resolved-sideband (κ ≪ ωₘ) and Doppler (κ ≫ ωₘ) cooling regimes
- Quantum limits of cooling as a function of cavity detuning
- Phase-space representation of thermal and cooled mechanical states

## Implementation Details

The simulation uses QuTiP's master equation solver to model the optomechanical system:

1. Phonon decay dynamics:
   - Implements Lindblad master equation with optomechanical coupling
   - Tracks average phonon number ⟨n⟩ over time
   - Compares cooling rates in different parameter regimes

2. Detuning optimization:
   - Scans laser-cavity detuning (Δ) to find optimal cooling conditions
   - Demonstrates different optimal detuning points for resolved vs. Doppler regimes
   - Quantifies final phonon occupancy as a function of system parameters

3. Wigner function visualization:
   - Computes phase-space distributions for initial thermal and final cooled states
   - Uses Gaussian approximations for clarity in visualization

## Performance Metrics

The simulation produces three key visualizations:

- **Phonon Decay Dynamics:**
  ![phonon_decay](phonon_decay.png)
  
  Shows cooling trajectories in different parameter regimes

- **Cooling Efficiency vs. Detuning:**
  ![cooling_vs_detuning](cooling_vs_detuning.png)
  
  Demonstrates optimal detuning conditions for minimal phonon occupancy

- **Wigner Function Comparison:**
  ![wigner_thermal_vs_cooled](wigner_thermal_vs_cooled.png)
  
  Visualizes the quantum state transformation from thermal (n ≈ 10) to cooled (n ≈ 0.5)

## References

F. Marquardt, J.P. Chen, A.A. Clerk, S.M. Girvin,
"Quantum Theory of Cavity-Assisted Sideband Cooling of Mechanical Motion",
Phys. Rev. Lett. 99, 093902 (2007)

## How to Run

```bash
conda activate qc-env
jupyter lab
```