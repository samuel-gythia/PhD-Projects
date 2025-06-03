# Microring Modulator Phase-Flip Demonstration

This simulation demonstrates how a microring resonator can be used to implement a quantum phase-flip operation through refractive index modulation, relevant for photonic quantum error correction schemes.

## Scientific Background

Photonic quantum computing requires reliable methods to manipulate quantum states. This simulation explores:

- Phase-flip operations (|1⟩→–|1⟩) in dual-rail encoded qubits
- Microring resonators as tunable phase modulators
- Relationship between refractive index changes and quantum phase shifts
- Applications in photonic quantum error correction schemes

## Implementation Details

The simulation uses a simplified analytical model:

1. The phase shift is modeled using a sinusoidal function of the refractive index change:
   ```
   η(Δn) = cos²(2π·Δn·L/λ)
   ```
   Where:
   - L = 2π·R is the ring circumference
   - λ is the wavelength of light
   - Δn is the change in refractive index

2. The model demonstrates:
   - Periodic behavior of transmission with refractive index change
   - Critical points where phase-flips occur (η = 0)
   - Optimal operating regions for phase modulation

## Performance Metrics

The simulation visualizes how transmission efficiency varies with refractive index change:

![ring_modulator_mock](ring_modulator_mock.png)

The plot shows:
- Complete extinction (η = 0) at specific Δn values, corresponding to perfect phase-flips
- Periodic behavior allowing for multiple operating points
- High sensitivity to small refractive index changes

## How to Run

```bash
conda activate qc-env
jupyter lab
```