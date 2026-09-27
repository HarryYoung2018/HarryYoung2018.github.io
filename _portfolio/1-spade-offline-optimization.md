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
- **Code:** [github.com/AAAAA-Academia-Attractions/SPADE](https://github.com/AAAAA-Academia-Attractions/SPADE)
- **Project page:** [aaaaa-academia-attractions.github.io/SPADE](https://aaaaa-academia-attractions.github.io/SPADE/)
- **Talk video:** [SlidesLive](https://slideslive.com/39075120/supportproximity-augmented-diffusion-estimation-for-offline-blackbox-optimization)
- **Stack:** Python, PyTorch, diffusion models, evolutionary search
