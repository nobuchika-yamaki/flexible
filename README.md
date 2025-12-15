# flexible
Flexible Control Framework (FCF)

This repository contains the core implementation of the Flexible Control Framework, a computational model showing how stability in redundant biological control systems can emerge from learning-driven reorganization of internal variability rather than increased control effort.

Contents
- core_model.py
  Implements the nonlinear redundant task, fixed-gain feedback control, learning-driven covariance reorganization, and computation of Compensatory Adjustment Capacity (CAC).
- simulation.py
  Runs single and multiple trials, computes task error, CAC, Jacobian sensitivity, and trial-wise correlations.
- figures/
  Scripts to reproduce main figures (Fig.1–3) from the manuscript.

Key concepts
- Task defined by a nonlinear mapping with redundancy.
- Stability achieved through redistribution of variability within task-equivalent subspaces.
- CAC quantifies compensatory flexibility as null-space variance.
- Feedback gain and noise amplitude are fixed throughout learning.

Requirements
- Python ≥ 3.9
- NumPy

Usage
1. Run a single trial:
   python core_model.py
2. Run multiple trials and summarize correlations:
   python simulation.py

Reproducibility
All simulations use fixed random seeds by default. Parameters (α, k, η, σ0, window size) are defined at the top of each script and correspond directly to the Methods section of the manuscript.

License
MIT License.

Contact
For questions related to the model or manuscript, contact the corresponding author.
