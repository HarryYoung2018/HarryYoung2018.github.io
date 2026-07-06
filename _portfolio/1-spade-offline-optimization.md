---
title: "SPADE — Diffusion Surrogates for Offline Optimization"
excerpt: "A calibrated conditional-diffusion surrogate with a kNN support prior for offline black-box optimization. Accepted to ICML 2026.<br/><em>PyTorch · diffusion models · optimization</em>"
collection: portfolio
---

**Support-Proximity Augmented Diffusion Estimation (SPADE)** models the forward likelihood
\\(p(y\mid x)\\) with a calibrated conditional diffusion model, then adds a k-nearest-neighbour
support prior so an offline optimizer cannot exploit regions the data never covered. It reaches
state-of-the-art results on Design-Bench and language-model optimization.

- **Venue:** ICML 2026 (co-first author) · ICLR 2026 DeLTa workshop
- **Paper:** [arXiv:2605.11246](https://arxiv.org/abs/2605.11246)
- **Code:** [github.com/HarryYoung2018/spade](https://github.com/HarryYoung2018/spade)
- **Project page:** [harryyoung2018.github.io/spade](https://harryyoung2018.github.io/spade/)
- **Stack:** Python, PyTorch, diffusion models, evolutionary search
