---
title: "Support-Proximity Augmented Diffusion Estimation for Offline Black-Box Optimization"
collection: publications
category: conferences
permalink: /publication/2026-spade-offline-black-box-optimization
excerpt: 'SPADE casts forward surrogate modeling as a calibrated conditional diffusion problem and adds a kNN support-proximity prior, so an offline optimizer stays expressive without exploiting unsupported, out-of-distribution regions. We prove the regularizer is equivalent to Bayesian inference under a valid design prior, and it tops Design-Bench and LLM-optimization tasks.'
date: 2026-05-01
venue: 'International Conference on Machine Learning (ICML)'
paperurl: 'https://arxiv.org/abs/2605.11246'
slidesurl: 'https://harryyoung2018.github.io/files/spade_icml2026_slides.pdf'
bibtexurl: 'https://harryyoung2018.github.io/files/spade_icml2026.bib'
citation: 'Yonghan Yang*, Ye Yuan*, Zipeng Sun, Linfeng Du, Bowei He, Haolun Wu, Can Chen, and Xue Liu. (2026). &quot;Support-Proximity Augmented Diffusion Estimation for Offline Black-Box Optimization.&quot; <i>Proceedings of the 43rd International Conference on Machine Learning (ICML 2026)</i>, PMLR 306, Seoul, South Korea. (* equal contribution)'
---

**ICML 2026** (Seoul, South Korea) · also accepted to the ICLR 2026
[DeLTa](https://openreview.net/forum?id=bTMCB3gorf) workshop · **my role: co-first author.**

<p>
  <a href="https://arxiv.org/abs/2605.11246" class="btn btn--info">Paper (arXiv)</a>
  <a href="https://harryyoung2018.github.io/spade/" class="btn btn--info">Project page</a>
  <a href="https://github.com/HarryYoung2018/spade" class="btn btn--info">Code</a>
  <a href="/files/spade_icml2026_slides.pdf" class="btn btn--info">Slides (PDF)</a>
  <a href="/files/spade_icml2026_slides.pptx" class="btn btn--info">Slides (PPTX)</a>
  <a href="/files/spade_icml2026_poster.pdf" class="btn btn--info">Poster</a>
</p>

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

## Slides

<div class="pdf-embed">
  <iframe src="/files/spade_icml2026_slides.pdf#view=FitH" title="SPADE ICML 2026 slides" loading="lazy"></iframe>
</div>
<p style="font-size:0.85em;"><em>Can't see the slides? <a href="/files/spade_icml2026_slides.pdf">Download the PDF</a> or the <a href="/files/spade_icml2026_slides.pptx">PPTX</a>.</em></p>

## Poster

<div class="pdf-embed pdf-embed--poster">
  <iframe src="/files/spade_icml2026_poster.pdf#view=FitH" title="SPADE ICML 2026 poster" loading="lazy"></iframe>
</div>
<p style="font-size:0.85em;"><em><a href="/files/spade_icml2026_poster.pdf">Download the poster (PDF)</a>.</em></p>

## BibTeX

```bibtex
@inproceedings{yang2026spade,
  title     = {Support-Proximity Augmented Diffusion Estimation for Offline Black-Box Optimization},
  author    = {Yang, Yonghan and Yuan, Ye and Sun, Zipeng and Du, Linfeng and
               He, Bowei and Wu, Haolun and Chen, Can and Liu, Xue},
  booktitle = {Proceedings of the 43rd International Conference on Machine Learning},
  series    = {Proceedings of Machine Learning Research},
  volume    = {306},
  address   = {Seoul, South Korea},
  publisher = {PMLR},
  year      = {2026}
}
```

<p style="font-size:0.85em;"><em><a href="/files/spade_icml2026.bib">Download .bib</a> (includes the arXiv entry).</em></p>

Work supervised by [Ye Yuan](https://stevenyuan666.github.io/) and
[Prof. Xue (Steve) Liu](https://cs.mcgill.ca/~xueliu/site/intro.html) at
[Mila – Quebec AI Institute](https://mila.quebec/en).
