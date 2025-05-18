\# Project: Coupling Efficiency in Si₃N₄ Waveguide–Microring Systems

This project explores coupling efficiency between a straight waveguide and a microring resonator using a simplified 2D photonic geometry. The structure is inspired by hybrid systems discussed in \*\*Lettner et al., ACS Photonics (2023)\*\*, which demonstrates precise dipole–cavity alignment for SiV centers in nanodiamonds coupled to Si₃N₄ photonic cavities.

\## Objective

To simulate and visualize how the waveguide–ring gap affects coupling efficiency in integrated photonic circuits. While this initial version uses a \*\*mock analytical model\*\* to demonstrate tunability, future iterations will incorporate \*\*full electromagnetic simulations\*\* using Meep or Tidy3D. (Tidy3D is used for our project.)

\## Plot

The output below shows exponential decay of coupling efficiency with increasing gap, emulating evanescent field overlap:

![coupling\_vs\_gap](coupling\_vs\_gap\_mock.png)

\## Reference

\> \*Lettner et al., "Hybrid SiV–nanodiamond–Si₃N₄ platform with full light–matter coupling control,"\* \*\*ACS Photonics\*\*, 2023.

\> https://arxiv.org/abs/2409.04252

\## To Run

\> bash

conda activate qc-env

jupyter lab
