# Project: Mock Vector Field Imaging with NV Probe

This demo simulates a planar scanning probe microscopy measurement of a 2D vector magnetic field,
mimicking techniques from Reinhard *et al.* (2024).

## Objective
Generate a mock vector field (radial pattern) and simulate NV-probe readings with noise.

## Method
- Create a uniform grid over ±5 µm.  
- Define true field ∝ (−y, x)/r.  
- Add Gaussian noise to emulate measurement uncertainty.  
- Use `matplotlib.streamplot` to visualize.

## Plot
![vector_field_scan](vector_field_scan_mock.png)

## Run
```bash
conda activate qc-env
jupyter lab
