---
layout: page
title: PADO-Pauli
description: GPU-accelerated, differentiable Pauli-propagation surrogate engine (Python package padopauli)
img: assets/img/pado_logo.png
importance: 1
---

[PADO-Pauli](https://github.com/Norma-Q/PADO-Pauli) is a Pauli-propagation surrogate (PPS) engine for simulating and training parameterized quantum circuits of 40–120 qubits, developed and maintained by Hyunwoo Kim and me at NORMA Inc. Instead of evolving a state vector, it propagates observables through the circuit in the Pauli basis and compiles the result into a reusable tensor program: compile once, then evaluate expectation values and gradients many times at different parameters.

- **Differentiable.** Expectation values are PyTorch tensors. Gradients flow to circuit parameters, and to classical layers feeding them, through a built-in manual VJP or host autograd.
- **GPU-accelerated.** `cpu`, `gpu`, and `hybrid` execution presets; the installed torch build (CUDA or ROCm) selects the device.
- **Compile once, evaluate many.** Batched parameters and data-embedding angles reuse the same compiled program; a quasi-sampler covers sampling workloads.
- **Noise-aware.** Depolarizing and amplitude-damping channels can be placed in the circuit.

The engine powers the surrogate pre-training in SAFE ma-QAOA and the large-scale experiments in our mixed IQP-QCBM work. Version 2.0.0 was released in September 2026. Presented as a poster at the Conference on Quantum Information (CQI 2026, Seoul) and accepted as a poster at IEEE Quantum Week 2026 (QCE26).

Links: [GitHub](https://github.com/Norma-Q/PADO-Pauli) · [PyPI](https://pypi.org/project/padopauli/) · [Zenodo DOI](https://doi.org/10.5281/zenodo.22627344)
