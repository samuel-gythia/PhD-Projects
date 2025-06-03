# NV-Center Ramsey Fringe Simulation

This simulation demonstrates Ramsey interference fringes in nitrogen-vacancy (NV) centers in diamond, providing a model for quantum coherence measurements in solid-state spin systems.

## Scientific Background

Ramsey interferometry is a fundamental technique for measuring quantum coherence times. In NV centers:

- The technique measures the phase accumulated during free evolution between two π/2 pulses
- Oscillations (fringes) appear due to detuning between the driving field and the spin transition
- Decay of fringe amplitude reveals the T₂* coherence time of the quantum system
- This coherence measurement is essential for quantum sensing and quantum information applications

## Implementation Details

The simulation uses a simplified analytical model:

1. The Ramsey signal is modeled as a damped oscillation:
   ```python
   signal = A * np.exp(-t/T2) * np.cos(2*np.pi*f*t + phase) + offset
   ```
   Where:
   - T₂ = 100 μs (decoherence time)
   - f = 1 MHz (fringe frequency, determined by detuning)
   - t = 0-200 μs (free evolution time)

2. The model demonstrates:
   - Oscillatory behavior due to Larmor precession during free evolution
   - Exponential decay envelope from decoherence processes
   - Complete signal extinction by approximately 3T₂

## Performance Metrics

The simulation visualizes the characteristic Ramsey interference pattern:

![ramsey_fringes_mock](ramsey_fringes_mock.png)

Key features shown in the plot:
- Oscillation frequency of 1 MHz corresponding to the detuning
- Decay envelope with T₂ = 100 μs
- Signal amplitude approaching zero after ~300 μs

## How to Run

```bash
conda activate qc-env
jupyter lab
open Reinhard_NV_Ramsey.ipynb
```