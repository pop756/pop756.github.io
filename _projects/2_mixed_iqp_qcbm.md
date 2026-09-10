---
layout: page
title: Mixed IQP-QCBMs
description: Trainability and mode separation of ancilla-extended IQP quantum generative models
importance: 2
---

IQP-based quantum circuit Born machines are attractive generative models because their MMD loss can be trained classically while sampling stays classically hard. Ancilla-free IQP circuits avoid barren plateaus under suitable initializations but are not universal; adding ancilla qubits restores expressivity but was not known to preserve trainability.

In [Trainability and Mode Separation of Mixed IQP-QCBMs](https://arxiv.org/abs/2607.27883) (Youngseok Lee and Hyunwoo Kim, arXiv:2607.27883), we view the ancilla-extended circuit as a weighted mixture of ancilla-free IQP circuits, called branches, that share one interaction graph but carry independent angles.

- We prove local barren-plateau avoidance for a polynomial number of branches under data-agnostic and, with assumptions, data-dependent initializations.
- A mixture surpasses the best ancilla-free circuit only if its branches generate distinct distributions. We call this **mode separation**, and show that branches started from the same distribution receive suppressed separating gradients.
- We propose **cluster initialization**, which seeds each branch from a different unsupervised data cluster, and show it converges fastest and reaches the lowest test MMD² on binary clusters, a 2D Ising model, binarized MNIST, and a 484-spin glass.

This work will be presented as a contributed talk at the ML4QT Symposium (University of Waterloo, September 2026).
