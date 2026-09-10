---
layout: page
title: Quantum generative models for molecules
description: Industry application of QGAN and IQP-QCBM models to drug-candidate generation, with experiments on real quantum hardware
importance: 4
---

At NORMA Inc. I applied quantum generative models to molecular generation for drug discovery, targeting candidate inhibitors of KRAS G12D.

- **Models.** Quantum GANs (including a PI-QGAN variant) and IQP-QCBMs trained on SMILES-derived representations and on the latent space of a classical autoencoder.
- **Hardware experiments.** Samples from trained generative models were drawn on Quantinuum H2, and their marginal distributions and correlations were compared against classical simulation. Related QAOA experiments were run on IonQ Forte.
- **Tooling.** The same Pauli-propagation surrogates that power PADO-Pauli were used to train and benchmark the circuits before deployment.

Ongoing follow-ups include noise-robust recovery of IQP/QCBM samples using classically computable low-order correlators (Ising priors, Bayesian denoising, and deconvolution), and a VQE study of nitrogen dissociation on Fe catalyst models.
