# Project 2: ML‑Enhanced Confidence Estimator (Synthetic Demo)

A purely synthetic proof-of-concept of Prof. Kraus’s ML‑augmented verification protocol.

## Overview
- **Features:** 4‑state probability vectors drawn from a Dirichlet distribution reflecting fidelity vs noise.
- **Labels:** 1 if fidelity ≥ 0.8; else 0.
- **Model:** Logistic Regression.
- **Accuracy vs Noise curve** ![accuracy_vs_noise](accuracy_vs_noise.png)
- **ROC CURVE** ![roc_curve](roc_curve.png)
## How to Run
```bash
conda activate qc-env
jupyter lab
