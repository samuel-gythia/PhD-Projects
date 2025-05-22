# PhD-Projects

This repository contains targeted demo projects developed as part of PhD outreach to selected faculty in quantum computing and simulation.  
Each folder corresponds to one professor and contains two concise research-aligned mockups, including Jupyter notebooks, plots, and READMEs.

## Project Index

### Prof. Benson – Hybrid Photonic Coupling
- [`Benson_FDTD/`](./Benson_FDTD): Mocked FDTD simulation of waveguide-ring coupling efficiency.
- [`Benson_RingModulator/`](./Benson_RingModulator): Tidy3D-inspired microring phase modulation demo.

### Prof. Reinhard – NV Center Probes
- [`Reinhard_VectorMapping/`](./Reinhard_VectorMapping): QuTiP simulation of Ramsey vector field mapping with NV centers.
- [`Reinhard_NV_Ramsey/`](./Reinhard_NV_Ramsey): Diamond probe design prototype for vector magnetometry (coming soon).

### Prof. Kraus – Clifford Verification & ML Confidence
- [`Kraus_CliffordVerifier/`](./Kraus_CliffordVerifier): Adaptive statistical protocol for distinguishing Clifford and non-Clifford gates.
- [`Kraus_MLConfidence/`](./Kraus_MLConfidence): ML classifier estimating circuit verification confidence under depolarizing noise.

### Prof. Bloch – Bose-Hubbard Mott Transition
- [`Bloch_MottTransition/`](./Bloch_MottTransition): 
  - 2-site ED spectrum vs U/J,
  - 4-site number fluctuation decay across Mott transition.

### Prof. Aidelsburger – Continuous Variable Squeezing
- [`Aidelsburger_CV/`](./Aidelsburger_CV): 
  - Single & two-mode squeezed vacuum simulations,
  - Cluster state Wigner reconstructions.

### Prof. Marquardt – Optomechanical Cooling
- [`Marquardt_Optomech/`](./Marquardt_Optomech): 
  - Sideband cooling vs Doppler regime,
  - Wigner plots of thermal vs cooled phonon states.

### Prof. Schwinger – Lattice Gauge Simulation
- [`Schwinger_Model/`](./Schwinger_Model):
  - Ground-state entanglement entropy vs. fermion mass.
  - Quench dynamics showing string breaking and gauge-matter oscillations.

---

## How to Run
Activate the environment and launch Jupyter Lab:
```bash
conda activate qc-env
jupyter lab