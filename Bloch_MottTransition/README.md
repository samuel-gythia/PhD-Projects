# Bloch_MottTransition

Reproduces key features of Bloch et al. (Nature 415, 39, 2002) superfluid–Mott transition  
in minimal Bose–Hubbard models.

## Project 1: 2‑Site Bose–Hubbard Spectrum
- Exact diagonalization for 2 bosons on 2 sites.
- Plot: `bloch_BH2_spectrum.png`.

## Project 2: 4‑Site Chain Number Fluctuations
- Exact diagonalization for 4 bosons on 4 sites.
- Compute ⟨n²⟩–⟨n⟩² vs. U/J for each site.
- Plot: `bloch_BH4_fluctuations.png`.

## Run
```bash
conda activate qc-env
jupyter lab