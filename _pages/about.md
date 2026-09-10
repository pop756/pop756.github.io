---
layout: about
title: about
permalink: /
subtitle: Quantum AI Developer · Quantum AI Team, <a href="https://www.norma.co.kr/">NORMA Inc.</a>

profile:
  align: right
  # image: prof_pic.jpg # add assets/img/prof_pic.jpg and uncomment this line
  image_circular: false
  more_info: >
    <p>Quantum AI Team</p>
    <p>NORMA Inc.</p>

selected_papers: true # includes a list of papers marked as "selected={true}"
social: true # includes social icons at the bottom of the page

announcements:
  enabled: true
  scrollable: true
  limit: 5

latest_posts:
  enabled: false
---

I am a quantum AI developer on the Quantum AI Team at NORMA Inc. I work on quantum machine learning and on the classical simulation tools needed to train it. My work follows three connected threads:

- **Quantum generative models.** Trainability and expressivity of IQP-based quantum circuit Born machines (QCBMs). In [Trainability and Mode Separation of Mixed IQP-QCBMs](https://arxiv.org/abs/2607.27883) (with Hyunwoo Kim), we generalize the ancilla-extended IQP circuit as a weighted mixture of ancilla-free branches, prove local barren-plateau avoidance, show that a mixture only helps when its branches separate into distinct modes, and propose a cluster initialization that seeds each branch from a different data cluster.
- **Variational quantum optimization.** SAFE ma-QAOA: classical pre-training of multi-angle QAOA with a Pauli-propagation surrogate, parameter distillation that prunes small angles, and exact fine-tuning, which together reduce the optimization cost of ma-QAOA. Accepted as a contributed talk at IEEE Quantum Week 2026 (QCE26).
- **GPU-accelerated quantum simulation.** I co-develop and maintain [PADO-Pauli](https://github.com/Norma-Q/PADO-Pauli), a GPU-accelerated, differentiable Pauli-propagation surrogate engine shipped as the Python package `padopauli`. It compiles a circuit once and then evaluates expectation values and gradients many times, so quantum circuits can be trained like any other PyTorch module. Accepted as a poster at QCE26.

On the applied side, I have built quantum generative models for molecular generation (QGAN and IQP-QCBM models over SMILES and autoencoder latent spaces, targeting KRAS G12D inhibitor candidates) and run such models on real hardware, including generative-model sampling on Quantinuum H2 and QAOA experiments on IonQ Forte. I am a co-inventor on two registered Korean patents (applicant: NORMA Inc.) on Pauli-graph surrogates for quantum circuit computation and quantum AI training, and I mentored a research intern on reinforcement learning for adaptive Pauli propagation.

Ongoing work includes noise-robust recovery of IQP/QCBM samples from classically computable low-order correlators, and connections between mixed IQP circuits and shared randomness in measurement-based quantum computation.

I received my B.S. in Nano Engineering from Sungkyunkwan University.

## upcoming talks

- **SAFE ma-QAOA** — contributed talk, [IEEE Quantum Week 2026 (QCE26)](https://qce.quantum.ieee.org/2026/), Toronto, September 13–18, 2026.
- **PADO-Pauli** — poster, [IEEE Quantum Week 2026 (QCE26)](https://qce.quantum.ieee.org/2026/), Toronto, September 13–18, 2026.
- **Trainability and Mode Separation of Mixed IQP Circuits** — contributed talk, [ML4QT Symposium](https://uwaterloo.ca/institute-for-quantum-computing/events/ml4qt-symposium-machine-learning-advance-quantum), Institute for Quantum Computing, University of Waterloo, September 23–25, 2026.
