---
title: "Support-Proximity Augmented Diffusion Estimation for Offline Black-Box Optimization"
collection: publications
category: conferences
permalink: /publication/2026-spade-offline-black-box-optimization
excerpt: 'SPADE casts forward surrogate modeling as a calibrated conditional diffusion problem and adds a kNN support-proximity prior, so an offline optimizer stays expressive without exploiting unsupported, out-of-distribution regions. We prove the regularizer is equivalent to Bayesian inference under a valid design prior, and it tops Design-Bench and LLM-optimization tasks.'
date: 2026-05-01
venue: 'International Conference on Machine Learning (ICML)'
paperurl: 'https://arxiv.org/abs/2605.11246'
citation: 'Yonghan Yang*, Ye Yuan*, Zipeng Sun, Linfeng Du, Bowei He, Haolun Wu, Can Chen, and Xue Liu. (2026). &quot;Support-Proximity Augmented Diffusion Estimation for Offline Black-Box Optimization.&quot; <i>International Conference on Machine Learning (ICML 2026)</i>. (* equal contribution)'
---

**Venue:** ICML 2026 · also accepted to the ICLR 2026 [DeLTa](https://openreview.net/forum?id=bTMCB3gorf) workshop
· **Role:** co-first author.

**Links:** [arXiv:2605.11246](https://arxiv.org/abs/2605.11246) ·
[code](https://github.com/HarryYoung2018/spade) ·
[project page](https://harryyoung2018.github.io/spade/)

## TL;DR

Offline black-box optimization searches for high-scoring designs from a fixed dataset with no
online oracle. The central failure mode is **out-of-distribution exploitation** — optimizers chase
surrogate errors in regions the data never covered. **SPADE** turns forward surrogate modeling into
a *calibrated conditional diffusion* problem and injects a **kNN support-proximity prior** that
shrinks predicted means and inflates uncertainty in low-density regions, keeping the search both
expressive and conservative.

## Contributions

- **Conditional diffusion surrogate** that models the forward likelihood \\(p_\theta(y\mid x)\\),
  yielding a predictive distribution rather than a point estimate.
- **Calibrated diffusion estimation** via moment matching and pairwise rank consistency, so the
  surrogate is actually useful for acquisition optimization.
- **Support-proximity regularization** using kNN density — which we prove is **equivalent to
  Bayesian inference under a valid design prior**.
- **State-of-the-art results** on Design-Bench and language-model optimization: mean rank 2.8/24
  and top-2 finishes on 5 of 6 tasks by normalized max score.

Work supervised by [Ye Yuan](https://stevenyuan666.github.io/) and
[Prof. Xue (Steve) Liu](https://cs.mcgill.ca/~xueliu/site/intro.html) at
[Mila – Quebec AI Institute](https://mila.quebec/en).
