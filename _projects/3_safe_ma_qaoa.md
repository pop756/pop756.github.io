---
layout: page
title: SAFE ma-QAOA
description: Surrogate-assisted, fine-tuning enhanced multi-angle QAOA with parameter distillation
importance: 3
---

Multi-angle QAOA (ma-QAOA) gives every gate its own angle, which improves approximation ratios but makes optimization expensive on hardware. SAFE ma-QAOA (Youngseok Lee and Hyunwoo Kim) reduces that cost in three stages:

1. **Surrogate pre-training.** A lightweight Pauli-propagation surrogate (LWPP) evaluates the ma-QAOA objective classically, so the initial optimization runs entirely off the quantum device.
2. **Parameter distillation.** Angles that stay small after pre-training are removed from the circuit, shrinking both the parameter count and the circuit depth.
3. **Exact fine-tuning.** The distilled circuit is fine-tuned with exact evaluation to recover any accuracy lost in the surrogate stage.

The method is accepted as a contributed talk at IEEE Quantum Week 2026 (QCE26), Toronto. A preprint link will be added when available.
